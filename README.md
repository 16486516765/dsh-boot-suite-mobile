# dsh-boot-suite 手机端移植版

把 LeeRolling/dsh-boot-suite v2.11.8 的**启动动画**移植到 DSHA 手机端（web profile，dsh 0.1.7）上用。动画本体（六幕、台词、CSS）未改，只改了安装与挂载方式。

- 原作者：沈宏宏，合并/维护：LeeRolling（MIT）
- 移植适配：zmjjkk
- 详细安装说明与真机验收清单：见 [MOBILE.md](MOBILE.md)

## 安装（手机端）

DSHA 里打开底栏「插件」页 → 「命令行安装」，粘贴：

```
dsh plugin --profile web add github:16486516765/dsh-boot-suite-mobile
```

然后重启 dsh，再进 WebUI 看启动动画。

## 注意

- 本仓库只含运行必需的文本文件（代码、模板 JSON、说明）。语音/音效等二进制素材（lib/assets、templates 各模板的 wav/mp3）因推送通道限制暂未随仓，装好后语音会回落到系统 TTS、音效回落到 WebAudio 合成，画面与时序不受影响；素材补齐后即恢复真声。
- 桌面版的安装.cmd、PowerShell 命令在手机上用不上，直接忽略。
- 聊天壁纸那半侧代码在仓内，但本版只保证启动动画在手机上能用，壁纸先别用。
