# Cloudflare Tunnel 文档站

[![Nuxt UI](https://img.shields.io/badge/Made%20with-Nuxt%20UI-00DC82?logo=nuxt&labelColor=020420)](https://ui.nuxt.com)

Cloudflare Tunnel 应用的官方文档站点，基于 Nuxt UI & Nuxt Content 构建。

在线地址：[https://tunnel.naspk.com/](https://tunnel.naspk.com/)

## 关于 Cloudflare Tunnel

Cloudflare Tunnel 是 fnOS 原生内网穿透应用，基于 Cloudflare 官方客户端适配。无需公网 IP、无需配置路由器端口转发，就能将 NAS、Web 面板、Home Assistant 等内网服务安全地暴露到互联网。

## 本地开发

```bash
pnpm install
```

```bash
pnpm dev
```

开发服务器启动后访问 `http://localhost:3000`。

## 构建部署

```bash
pnpm build
```

```bash
pnpm preview
```

## 技术栈

- [Nuxt 4](https://nuxt.com)
- [Nuxt UI](https://ui.nuxt.com)
- [Nuxt Content](https://content.nuxt.com)

## 许可证

[MIT](./LICENSE)