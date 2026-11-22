# 第三方组件

此 Windows 下载版随附未修改的 Electron 45.3.2 运行组件，并保留 Electron 与 Chromium 的许可证和第三方声明。官方运行组件、对应源代码及构建配置可从 [Electron v45.3.2](https://github.com/electron/electron/releases/tag/v45.3.2) 获取。[Electron 依赖清单](https://github.com/electron/electron/blob/v45.3.2/DEPS) 固定了 [Chromium 156.0.8078.100](https://chromium.googlesource.com/chromium/src/+/refs/tags/156.0.8078.100) 的源代码版本。Chromium 的 DEPS 同时固定播放器所用 FFmpeg 动态库的源码。对应的 Electron 发布构建参数位于 [release.gn](https://github.com/electron/electron/blob/v45.3.2/build/args/release.gn)。Electron 自带的播放器运行组件与下文的独立 FFmpeg 工具分开。

应用使用 React、React DOM、SQL.js、Chokidar、Cheerio 和 Unzipper。各组件的许可随其分发内容提供。

## 可选的独立媒体组件

`Install-FFmpeg.cmd` 供用户自行从 [Gyan FFmpeg Essentials 9.0.2 官方发布](https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2) 安装两个独立命令行工具。该下载由上游提供，版本及 SHA-256 在安装脚本中固定。Gyan 将该构建按 GPLv3 发布，其许可证与构建说明保留在安装组件的目录内。FFmpeg 项目上游源码版本为 [946fcce07b](https://github.com/FFmpeg/FFmpeg/commit/946fcce07b)。
