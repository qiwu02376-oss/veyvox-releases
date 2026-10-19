# Veyvox

本地课堂语音识别与中文翻译助手，无需终端或 API Key。

## 下载修正版

[下载 Veyvox 0.4.2 beta.1（Apple Silicon Mac）](https://github.com/qiwu02376-oss/veyvox-releases/releases/tag/v0.4.2-beta.1)

在发布页选择 `Veyvox-0.4.2-beta.1-macOS-arm64.dmg`。0.4.1 beta.1 的安装包存在完整性问题，请改用 0.4.2。

## 安装

1. 打开 DMG，将 Veyvox.app 拖到「应用程序」，再打开。
2. 在「配置指引 → AI Engine」安装 Moonshine 和 Qwen3（约 3 GB），点击「检测本地模型」。
3. 检测通过后允许麦克风并开始翻译。首次下载需要联网，之后识别和翻译在本机运行。

## 要求与限制

- 仅支持 Apple Silicon（M 系列）Mac，建议 16 GB 或更多内存及至少 8 GB 可用磁盘空间。
- 构建目标 macOS 15+；实测 macOS 27.0.1，macOS 15/26 和 8 GB 内存机型尚未实机验证。
- 测试版尚无 Apple Developer ID 签名与公证。若被阻止首次打开，请确认来自本仓库，再按 [Apple 官方说明](https://support.apple.com/102445) 在「隐私与安全性」选择「仍要打开」。
- 远场、噪声和多人讲话可能造成漏词、误译或延迟。关闭窗口保留后台服务，完全退出请用菜单「退出 Veyvox」。

详细安装说明见 [INSTALL-zh.txt](INSTALL-zh.txt)。本仓库分发安装包，GitHub 自动生成的 Source code 不是应用源码。
