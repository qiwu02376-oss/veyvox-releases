# Orva（原 Veyvox）

macOS 本地语音识别、双语字幕与课堂学习助手。Orva 0.6.0 beta.1 是 Veyvox 0.4.2 的后续版本，本仓库地址保留以兼容原下载链接。

## 下载最新版

**[下载 Orva 0.6.0 beta.1 · Apple Silicon Mac 安装包](https://github.com/qiwu02376-oss/veyvox-releases/releases/download/v0.6.0-beta.1/Orva-0.6.0-beta.1-macOS-arm64.dmg)**

[发布说明与 SHA256 校验文件](https://github.com/qiwu02376-oss/veyvox-releases/releases/tag/v0.6.0-beta.1)。请下载 `.dmg`，GitHub 自动生成的 Source code 压缩包不是 App。

## 首次使用

1. 把 Orva.app 拖到「应用程序」，再打开。
2. 在「连接与配置 → AI Engine」下载需要的模型：英语用 Parakeet；其他七种源语言用 Whisper small 多语言；翻译建议选择并安装 Index-Translate。原 Qwen3 英译中选项保留。
3. 在主界面选择源语言和目标语言，确认正确的音频输入和转写许可后开始。下载模型需要联网，安装后的本地识别和翻译无需 API Key，可离线运行。

详细说明：[INSTALL-zh.txt](INSTALL-zh.txt)。

## 这一版的变化

- 手动选择英语、简体中文（普通话）、西班牙语、日语、韩语、法语、德语、俄语，并可交换源语言与目标语言。
- 保留英语 Parakeet，引入本地 Whisper small 多语言；按当前源语言检查所需模型。
- 字幕原文/译文配对，支持上下、宽屏双栏和悬浮字幕；改进历史回看和返回实时。
- 保留课堂记录、导出和 AI 笔记；改善模型切换、重启后的配置恢复及异常响应保护。
- 四个本地翻译选项和原三个云端选项保留。语言方向、安装状态和费用资格分别检查；不会自动更换翻译 Provider。

## 测试范围与限制

325 项单元/集成测试、37 项浏览器测试通过，4 项需单独启用的专项测试跳过。八个方向已用真实本地模型处理合成短语音；十分钟循环普通话测试完成 111 段翻译。这不代表真人课堂准确率验收通过。

自动语言检测暂未开启。日语术语、俄语专业译法及强制切段处仍可能识别或翻译不准；噪声、远场、多人讲话也会影响结果。Qwen3 主要保留已验证英译中；TranslateGemma 非英语互译尚未开放；Google NMT 仍处费用保护状态。

本地路径无 API 费用。主动选择云端服务后，Qwen-MT 可按量收费（默认 ¥10/月为提醒，并非硬上限）；DeepL 只允许经验证的 Free 资格，额度用尽即停止。安装包不包含 API Key。

## 系统与升级

Apple Silicon（M 系列）Mac，构建目标 macOS 15+，已在 M4 / 16 GB 测试。建议至少 16 GB 内存并预留 10 GB 以上给 App、模型和录音。Intel、Windows、手机及 8 GB 内存机型未验证或不支持。

此版本使用本地签名，**尚无 Apple Developer ID 签名与公证**。如被 macOS 阻止首次打开，请确认来自本仓库，再按 [Apple 官方说明](https://support.apple.com/102445) 操作。

升级前完全退出旧 App，再替换应用程序；保留 `~/Library/Application Support/Orva` 及旧 Veyvox 数据目录，确认记录迁移后再处理旧 App。自动更新尚未实现，后续版本从本仓库手动下载安装。

旧版发布保留作回退：[所有版本](https://github.com/qiwu02376-oss/veyvox-releases/releases)。反馈请提供芯片、内存、系统版本和复现步骤，不要公开上传私人课堂资料或密钥。
