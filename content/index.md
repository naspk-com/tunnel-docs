---
title: Cloudflare Tunnel
description: 无需公网 IP，无需配置复杂路由。通过 Cloudflare 边缘网络，安全、快速地将你的 fnOS 服务暴露到互联网。
image:
  light: /images/hero-light.png
  dark: /images/hero-dark.png
links:
  - label: 快速开始
    to: /quickstart
    icon: i-lucide-rocket
  - label: API 接入
    to: /advanced/api-credentials
    icon: i-lucide-key
  - label: SDK 下载
    to: /advanced/sdk
    icon: i-lucide-download
  - label: 加入 QQ 群聊
    to: https://qm.qq.com/q/AF0rPKcHde
    target: _blank
    icon: i-lucide-users
features:
  - title: 无需公网 IP
    description: 即使你的宽带没有分配公网 IPv4，也能通过 Cloudflare 边缘网络轻松实现外网访问。
    icon: i-lucide-network
  - title: 安全加密
    description: 所有流量通过 Cloudflare 全球网络加密传输，隐藏真实 IP，原生防御 DDoS 攻击。
    icon: i-lucide-shield-check
  - title: API 集成
    description: 提供 RESTful API、MCP 服务和多语言 SDK，方便其他应用和 AI 智能体集成 Tunnel 管理能力。
    icon: i-lucide-code
quickLinks:
  - title: 快速开始
    description: 了解功能概览，三步完成首个 Tunnel 配置。
    to: /quickstart
    icon: i-lucide-rocket
  - title: 配置指南
    description: 配置 Cloudflare 账号凭据与系统连接参数。
    to: /configuration/cloudflare-credentials
    icon: i-lucide-key
  - title: Tunnel 管理
    description: 创建、连接、配置域名转发规则。
    to: /tunnel-management/manage-tunnels
    icon: i-lucide-list
  - title: API 凭证与 SDK
    description: 获取 API 凭证、下载 SDK，将 Tunnel 集成到你的应用中。
    to: /advanced/api-credentials
    icon: i-lucide-code
  - title: 帮助排障
    description: 常见问题解答与故障排除指南。
    to: /help/troubleshooting
    icon: i-lucide-life-buoy
---

## 什么是 Cloudflare Tunnel？

Cloudflare Tunnel 通过 Cloudflare 全球边缘网络，在你的 fnOS 设备和外部互联网之间建立一条安全隧道。你无需公网 IP、无需配置路由器端口转发，即可让你的 fnOS 服务（如 [QwenPaw](/products/qwenpaw)、[It-Tools](/products/it-tools) 等）安全地暴露到互联网。

![功能概览](/images/hero-light.png)

## 核心功能

- **Tunnel 管理**：创建、启动、停止 Cloudflare Tunnel，支持多个 Tunnel 之间快速切换
- **域名转发**：为第三方应用注册独立域名，自动配置 DNS 和 ingress 规则
- **API 凭证**：创建 API 凭证，支持外部应用通过独立 HTTP API 调用 Tunnel 管理接口
- **MCP 服务**：内置 MCP（Model Context Protocol）服务，可将全部 Tunnel 管理能力暴露给 AI 智能体（如 QwenPaw、OpenClaw 等）
- **多语言 SDK**：提供 Python、JavaScript/TypeScript、Go、Shell 四种 SDK，开箱即用
- **日志查看**：内置 Tunnel 运行日志，方便排障

## 适用场景

| 场景 | 说明 |
|------|------|
| 部署 QwenPaw 等 AI 服务 | 将本地运行的 AI 模型通过独立域名对外提供服务 |
| 搭建个人网站或工具 | 让 [It-Tools](/products/it-tools)、[fnDesign](/products/fndesign) 等服务可通过公网访问 |
| 远程访问 NAS | 在外网安全地访问 fnOS 上的文件服务 |
| 应用间集成 | 通过 API/SDK 让其他应用自动管理 Tunnel 域名 |