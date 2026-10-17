# Veyvox

离线课堂同声传译：把英文讲课实时转成中文字幕，语音识别和翻译都在本机运行，不需要 API Key。

## 下载

👉 到 [Releases](https://github.com/qiwu02376-oss/veyvox-releases/releases/latest) 下载最新的 `Veyvox-*-macOS-arm64.dmg`。

## 系统要求

- Apple Silicon（M 系列）Mac，macOS 15 或更高
- 建议 16 GB 内存，至少 8 GB 可用磁盘空间
- 不支持 Intel Mac、Windows 或手机

## 安装

1. 打开 DMG，把 Veyvox 拖到「应用程序」。
2. 第一次打开如果提示「无法验证开发者」：到「系统设置 → 隐私与安全性」点「仍要打开」（或在应用程序里右键 Veyvox 选「打开」）。这是因为测试版还没有 Apple 签名。
3. 在 App 的「配置指引」里安装 Moonshine 和 Qwen3 模型（约 3 GB），点「检测本地模型」，允许麦克风后开始翻译。

详细说明见 [INSTALL-zh.txt](INSTALL-zh.txt)。

## 说明

这是测试版，识别和翻译在远场、噪声或多人讲话时可能漏词或误译。欢迎在 Issues 里反馈。
