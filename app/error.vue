<script setup lang="ts">
import type { NuxtError } from '#app'

defineProps<{
  error: NuxtError
}>()

useHead({
  htmlAttrs: {
    lang: 'en'
  }
})

useSeoMeta({
  title: '飞牛Cloudflare Tunnel - Page not found',
  description: '很遗憾，页面不存在。'
})

const { data: navigation } = await useAsyncData('navigation', () => queryCollectionNavigation('docs' as never))
const { data: files } = useLazyAsyncData('search', () => queryCollectionSearchSections('docs' as never), {
  server: false
})

provide('navigation', navigation)
</script>

<template>
  <UApp>
    <AppHeader />

    <UError :error="error" />

    <AppFooter />

    <ClientOnly>
      <LazyUContentSearch
        :files="files"
        :navigation="navigation"
      />
    </ClientOnly>
  </UApp>
</template>
