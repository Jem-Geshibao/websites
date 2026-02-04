# Rikka Apps — 网站文档集合

本仓库存放 Rikka Apps 各项目的静态网站源代码（基于 VuePress），包括但不限于：
- Shizuku
- App Ops
- Storage Redirect
- 官方聚合站（rikka.app）

文档支持中文（简体/繁体）与英文等多语言，并使用 Weblate 进行翻译协作。

---

## 📦 快速开始

先确保已安装 Node.js 与 npm，然后在仓库根目录运行：

```bash
npm install
```

常用命令（在 package.json 中已有定义）：

- 本地开发（自动热重载）：
  - `npm run shizuku:dev` — 启动 Shizuku 文档
  - `npm run appops:dev` — 启动 App Ops 文档
  - `npm run sr:dev` — 启动 Storage Redirect 文档
  - `npm run www:dev` — 启动主站文档

- 构建静态文件：
  - `npm run shizuku:build` / `npm run appops:build` / `npm run sr:build` / `npm run www:build`

构建后的静态文件会输出到相应站点目录下的 VuePress 输出目录（例如 `<site>/.vuepress/dist`）。

> 提示：如需预览已构建的静态站点，可使用任何静态文件服务器（例如 `npx serve <dist-dir>`）。

---

## 🗂 目录概览

仓库中的主要目录：

- `shizuku/` — Shizuku 文档站点
- `appops/` — App Ops 文档站点
- `storage_redirect/` — Storage Redirect 文档站点
- `www/` — 官方聚合与通用内容（隐私、翻译指引等）
- `webhooks/` — 与构建/部署相关的简单 Webhook 脚本

各子目录通常包含多语言版本：`zh-hans/`（简体）、`zh-hant/`（繁体）以及默认英文内容。

---

## 🤝 贡献

- 翻译：使用 Weblate 平台（https://weblate.rikka.app/）参与翻译。详见 `www/contribute_translation.md`。
- 文档/内容变更：直接在仓库中提交 Issue 或 PR，仓库地址：https://github.com/RikkaApps/websites
- 特定项目（例如 Storage Redirect）的贡献规则、数据提交说明等请参见对应子项目下的 `guide/contribute.md`。

---

## ⚖️ 许可与第三方信息

本仓库使用 VuePress 及其主题，其中部分主题/组件受 MIT 许可（参见 `storage_redirect/.vuepress/theme/LICENSE`）。
各应用（Shizuku、App Ops、Storage Redirect 等）为独立项目，请参阅它们各自的代码仓库与许可证声明：
- Shizuku: https://github.com/RikkaApps/Shizuku
- 其他仓库请在文档中查找对应链接。

---

## 📬 联系与支持

- 反馈/问题: 提交 GitHub Issue 或发送邮件到 `support@rikka.app`（在某些文档中可见）。
