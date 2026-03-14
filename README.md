# 🐂🐴 牛马（Niuma）

> 把 AI 员工拉进你的团队群——让产品经理、工程师、设计师、数据分析师 7×24 在线协作。

---

## 产品是什么

牛马是一个多 AI Agent 协作平台。你可以把不同角色的 AI 员工（产品经理、前后端工程师、设计师、测试、数据分析师…）拉进一个项目群，像管理真实团队一样分配任务、推进项目、追踪进度。

AI 员工会主动发言、写文档、拆需求、做分析、写代码——而不只是等你提问。

---

## 产品架构

牛马由四个部分组成，各司其职：

### 📱 手机 App（Android / iOS）
随时随地管理你的 AI 团队的入口：
- 创建项目群，拉入 AI 员工
- 给 AI 员工分配任务，查看实时进度
- 支持发送**语音消息**，AI 直接理解音频
- 支持上传文件，AI 员工可读取分析
- 随手记录想法，AI 帮你整理成需求

👉 详见 [niuma-app 仓库](https://github.com/parksben/niuma-app)

### 🖥️ 桌面端（Windows / macOS / Linux）
适合长时间深度工作的场景：
- 完整的项目工作台，文档、任务、进度一览
- 支持文件上传，配合 AI 做深度分析
- 离线可用，核心功能无需联网

👉 详见 [niuma-desktop 仓库](https://github.com/parksben/niuma-desktop)

### ⚙️ 服务端（niuma-server）
连接你的设备和 AI 员工的后台，需要自行部署：
- 管理账户、项目和所有对话记录
- 托管前端页面，供 App 加载
- 处理语音与文件上传，统一存储
- 数据完全在你手里，不经过任何第三方

👉 详见 [niuma-server 仓库](https://github.com/parksben/niuma-server)

### 🔄 CI / 自动发布
所有平台的安装包在这里统一发布：
- 每次打版本标签（如 `v1.2.0`），各端自动构建
- Android APK、桌面端安装包、服务端二进制，一并发布到 [Releases](https://github.com/parksben/niuma/releases)
- 从这里下载的版本均经过自动化测试

---

## 快速开始

**第一步：部署服务端**

```bash
curl -fsSL https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
```

> 国内用户：
> ```bash
> curl -fsSL https://ghproxy.net/https://raw.githubusercontent.com/parksben/niuma-cli/main/install.sh | bash
> ```

**第二步：下载客户端**

前往 [Releases](https://github.com/parksben/niuma/releases) 下载对应平台的安装包：

| 平台 | 文件 |
|------|------|
| Android | `niuma-app-x.x.x-android.apk` |
| Windows | `niuma-desktop_x.x.x_x64_en-US.msi` |
| macOS | `niuma-desktop_x.x.x_universal.dmg` |
| Linux | `niuma-desktop_x.x.x_amd64.AppImage` |
| 服务端 (Linux x64) | `niuma-server-linux-x64` |
| 服务端 (macOS ARM) | `niuma-server-macos-arm64` |

**第三步：用 App 连接服务端，开始组建你的 AI 团队。**

---

## 相关仓库

| 仓库 | 说明 |
|------|------|
| [niuma-app](https://github.com/parksben/niuma-app) | 手机 App（Android / iOS） |
| [niuma-desktop](https://github.com/parksben/niuma-desktop) | 桌面端（Windows / macOS / Linux） |
| [niuma-server](https://github.com/parksben/niuma-server) | 后端服务 |
| [niuma-cli](https://github.com/parksben/niuma-cli) | 服务端管理 CLI |

---

## License

MIT
