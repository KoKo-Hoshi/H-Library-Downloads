# H Library 私人影音库 Windows 下载

H Library 是一款借助 OpenAI Codex 实现的管理小姐姐和老师们视频的私人本地影音库库，支持整理本地媒体、标签筛选、收藏、播放和 AI 资料补全。安装包带 13 个离线体验样本，安装后可在设置中切换到体验库。

## 下载和安装

1. 在 [最新版本](https://github.com/KoKo-Hoshi/H-Library-Downloads/releases/latest) 的 **Assets** 中下载 `H-Library-2.3.2-Windows-x64-Setup.exe`，运行安装向导。适用于 Windows 10/11 64 位。
2. 需要读取本地媒体时长、自动提取封面或从视频抽帧时，打开安装目录，双击 `Install-FFmpeg.cmd`，按提示输入 `Y`。该脚本从 Gyan 的上游发布页下载约 110 MB 的 FFmpeg Essentials 9.0.2，并校验 SHA-256。完成后重启 H Library。

如果脚本无法下载，可以从 [上游发布页](https://github.com/GyanD/codexffmpeg/releases/tag/9.0.2) 下载 `ffmpeg-9.0.2-essentials_build.zip`，解压后将 `bin` 里的 `ffmpeg.exe`、`ffprobe.exe` 与包内的 `LICENSE`、`README.txt` 放入 H Library 安装目录的 `resources\ffmpeg\`。目录不存在时可手动创建。

安装包未签名。版本页提供 SHA-256，可用来核对下载的文件。

## 数据与第三方组件

H Library 将媒体库索引、收藏和观看进度存到本机。软件内联网补全为可选功能，需要自行配置模型服务。公开下载包包含软件和离线体验素材。

随包提供 Electron 和 Chromium 的许可文件。Gyan 的 FFmpeg 和 FFprobe 由其上游单独提供。

第三方组件的版本和源码链接见 [第三方说明](THIRD_PARTY.md)。
