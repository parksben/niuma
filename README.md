# 🐂🐴 牛马（Niuma）

> AI 驱动的多 Agent 协作平台 —— 让你的产品团队随时在线。

## 下载

前往 [**Releases**](https://github.com/parksben/niuma/releases) 下载最新版本。

| 平台 | 文件 |
|------|------|
| Android | `.apk` |
| iOS | `.ipa`（需自签或 TestFlight） |
| Windows | `.exe` 安装包 |
| macOS | `.dmg` |
| Linux | `.AppImage` |

---

## 项目介绍

牛马是一个基于 [OpenClaw](https://openclaw.ai) 的多 Agent 协作系统，支持创建 AI 员工团队，自动完成产品规划、开发、设计、分析等工作。

你可以在 App 或桌面端创建「产品项目」，拉入不同角色的 AI 员工（规划师、工程师、设计师、分析师…），让他们在群聊里协作完成任务。

---

## 部署服务端

使用 App 或桌面端前，需要先自行部署 niuma-server。执行以下命令，按向导一键完成部署：

```bash
curl -fsSL https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
```

> 国内用户推荐：
> ```bash
> curl -fsSL https://ghproxy.net/https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
> ```

**系统要求：**
- Linux / macOS 服务器
- Node.js 18+
- 已安装 [OpenClaw](https://openclaw.ai)

---

## 产品架构

```
┌─────────────────────────────────────────────────┐
│               用户端                             │
│  niuma-app (iOS / Android)                       │
│  niuma-desktop (Windows / macOS / Linux)         │
└────────────────────┬────────────────────────────┘
                     │ HTTP / SSE
┌────────────────────▼────────────────────────────┐
│               niuma-server                       │
│  用户认证 · 项目管理 · Agent 路由 · 消息持久化   │
└────────────────────┬────────────────────────────┘
                     │ OpenClaw API
┌────────────────────▼────────────────────────────┐
│               OpenClaw                           │
│  多 Agent 运行时 · 工具调用 · 记忆 · 定时任务   │
└─────────────────────────────────────────────────┘
```

---

## 技术栈

| 端 | 技术 |
|----|------|
| 移动端 | React Native |
| 桌面端 | Tauri + React |
| 前端 WebView | React + Vite + TypeScript |
| 服务端 | Node.js + Express + SQLite |
| AI 运行时 | OpenClaw Agent 框架 |
| 认证 | 邮箱 OTP + JWT |

---

## 相关工具

- [niuma-cli](https://github.com/parksben/niuma-cli) — 服务端一键安装命令行工具

---

## License

MIT
