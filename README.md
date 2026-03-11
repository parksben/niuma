# 🐂🐴 牛马（Niuma）

> AI 驱动的多 Agent 协作平台，让你的产品团队随时在线。

## 下载 App

前往 [**Releases**](https://github.com/parksben/niuma/releases) 下载最新版本 APK。

| 版本 | 说明 |
|------|------|
| [最新版本](https://github.com/parksben/niuma/releases/latest) | 点击下载最新 APK |

**安装方法：**
1. 下载 `.apk` 文件
2. Android 手机开启「允许安装未知来源应用」
3. 安装 APK，启动即可

---

## 项目介绍

牛马是一个基于 [OpenClaw](https://openclaw.ai) 的多 Agent 协作系统，支持创建 AI 员工团队，自动完成产品规划、开发、设计、分析等工作。

你可以在 App 里创建「产品项目」，拉入不同角色的 AI 员工（规划师、工程师、设计师、分析师…），让他们在群聊里协作完成任务。

---

## 产品组件

| 组件 | 说明 | 仓库 |
|------|------|------|
| 牛马 App | Android / iOS 客户端（Flutter） | 本仓库 Releases |
| [niuma-server](https://github.com/parksben/niuma-server) | 后端服务（Node.js + SQLite） | 开源 |
| [niuma-cli](https://github.com/parksben/niuma-cli) | 命令行安装工具 | 开源 |

---

## 部署服务端

用户需要自行部署 niuma-server 才能使用 App。执行以下命令，按向导完成一键部署：

```bash
curl -fsSL https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
```

**系统要求：**
- Linux 服务器（Ubuntu / CentOS）
- Node.js 18+
- 已安装 [OpenClaw](https://openclaw.ai)

---

## 技术栈

- **App**: Flutter（Android-first，跨平台）
- **Server**: Node.js + Express + SQLite
- **AI**: OpenClaw Agent 框架
- **Auth**: 邮箱 OTP + JWT

---

## License

MIT
