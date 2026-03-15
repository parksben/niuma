# 🐂🐴 牛马（Niuma）

> AI 驱动的多 Agent 协作平台 —— 让你的产品团队随时在线。

## 产品介绍

牛马是一个基于 [OpenClaw](https://openclaw.ai) 的多 Agent 协作系统，支持创建 AI 员工团队，自动完成产品规划、开发、设计、分析等工作。

在 App 或桌面端创建「产品项目」，拉入不同角色的 AI 员工（规划师、工程师、设计师、分析师…），让他们在群聊里协作完成任务。

---

## 快速开始

### 1. 部署服务端

```bash
curl -fsSL https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
```

> 国内用户推荐：
> ```bash
> curl -fsSL https://ghproxy.net/https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
> ```

安装完成后按照终端提示启动服务，在配置页面填入 OpenClaw Token 即可。

### 2. 下载客户端

前往 [**Releases**](https://github.com/parksben/niuma/releases) 下载最新版本：

| 平台 | 文件 |
|------|------|
| Android | `.apk` |
| Windows | `.exe` 安装包 |
| macOS | `.dmg` |
| Linux | `.AppImage` |

> iOS 版正在开发中，敬请期待。

### 3. 连接服务

打开客户端 → 输入你的服务地址 → 登录即可使用。

---

## 产品架构

```
┌─────────────────────────────────────────────────┐
│               用户端                             │
│  App (Android)  ·  Desktop (Win / Mac / Linux)  │
└────────────────────┬────────────────────────────┘
                     │ HTTP / SSE
┌────────────────────▼────────────────────────────┐
│               牛马服务端                         │
│  用户认证 · 项目管理 · Agent 路由 · 消息持久化   │
└────────────────────┬────────────────────────────┘
                     │ OpenClaw API
┌────────────────────▼────────────────────────────┐
│               OpenClaw                           │
│  多 Agent 运行时 · 工具调用 · 记忆 · 定时任务   │
└─────────────────────────────────────────────────┘
```

---

## 系统要求

- Linux / macOS 服务器（用于部署服务端）
- 已部署 [OpenClaw](https://openclaw.ai)

---

## License

MIT
