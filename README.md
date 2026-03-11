# 🐂🐴 牛马（Niuma）

> AI 驱动的多 Agent 协作平台，让你的产品团队随时在线。

## 项目介绍

牛马是一个基于 OpenClaw 的多 Agent 协作系统，支持创建 AI 员工团队，自动完成产品规划、开发、设计、分析等工作。

## 产品组件

| 组件 | 说明 | 仓库 |
|------|------|------|
| 牛马 App | Android / iOS 客户端（Flutter） | 私有 |
| [niuma-server](https://github.com/parksben/niuma-server) | 后端服务（Node.js + SQLite） | 开源 |
| [niuma-cli](https://github.com/parksben/niuma-cli) | 命令行安装工具 | 开源 |

## 快速开始

### 部署服务端

```bash
curl -fsSL https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
```

### 下载 App

前往 [Releases](https://github.com/parksben/niuma-app/releases) 下载最新 APK。

## 技术栈

- **App**: Flutter（Android-first，跨平台）
- **Server**: Node.js + Express + SQLite
- **AI**: OpenClaw Agent 框架
- **Auth**: 邮箱 OTP + JWT

## License

MIT
