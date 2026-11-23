# Free Auto CarPlay

让 Android 4.0 及以上的车机用上 CarPlay：通过外置 USB 蓝牙接收器或车机自带蓝牙连接 iPhone，不需要改装车机，也不需要 root。

> 本项目基于 Display 与 XcertPlay 修改而来，自 2026-10-01 起开发，按 [AGPL-3.0](LICENSE) 发布。

## 下载

所有版本都在 [Releases](https://github.com/Free-Auto-Car/Free-Auto-Carplay/releases) 页面，最新正式版为 **v1.4.9**。

安装包为 32 位（`armeabi-v7a`），适用于 Android 4.0–9 的车机。旧版车机装不上或黑屏时，先升级到最新版本再试。

## 支持的连接方式

| 方式 | 说明 |
|---|---|
| 外置 USB 蓝牙接收器 | 车机没有可用蓝牙时使用，插上即可；应用内可查看接收器状态并授权 |
| 车机自带蓝牙 | 车机蓝牙可正常配对 iPhone 时使用 |
| 有线 | 通过 USB 连接 iPhone，不依赖蓝牙 |

连接路线由首次引导选定，之后按「外置蓝牙只走接收器、车机蓝牙只走车机蓝牙」执行。

## 特性

- **首次引导**：检测车机能力、选连接方式、配对、视频、声音、麦克风、USB 供电逐项实测，按结果确定配置。
- **连接流程**：点「连接」后留在主界面，画面就绪自动进入 CarPlay；断开后不自动重连。
- **外置蓝牙**：开启后强制占用接收器，拔插后自动恢复，不影响其他应用的默认设置。
- **在线更新**：应用内检查更新，更新包可不经过完整重新安装直接生效；设置、配对、引导进度、首页图片都会保留。
- **方向盘按键学习**：Android 4.x 车机可用。
- **诊断**：日志导出合成单个文件，断电不丢记录；崩溃自动记录。

## 安装

1. 从 [Releases](https://github.com/Free-Auto-Car/Free-Auto-Carplay/releases) 下载对应版本的 APK。
2. 在车机上安装（需要允许「未知来源」）。
3. 首次启动会进入引导，按屏幕提示逐项完成检测。

## 版本

| 版本 | 日期 | 要点 |
|---|---|---|
| v1.0.0 | 2026-10-08 | 首个版本，新的连接流程、外置 USB 蓝牙、应用内升级 |
| v1.0.1 | 2026-10-10 | 修复版：诊断脱敏、崩溃落盘、热点改名不再改密码 |
| v1.0.2 | — | 内部修复版，未作为正式版本发布 |
| v1.1.0 | 2026-10-12 | 已连接时重新打开直接进入；启动按 USB 判断连接路线；外观自动；帧率 60 |
| v1.2.0 – v1.2.4 | 2026-10-13 – 10-14 | 有线链路移植与修复、外置蓝牙保持连接、Android 4.x 兼容修复 |
| v1.2.5 | — | 由另一条工作线发布，本仓库无对应说明 |
| v1.3.0 – v1.3.4 | 2026-10-19 – 10-24 | 首次引导向导、连接路线强制、解码与黑屏修复、USB 供电测试、音频优先级 |
| v1.4.0 – v1.4.9 | 2026-11 | 在线更新、外置蓝牙与无线连接改进、热更新 |

每个版本的完整更新说明见对应的 Release。

## 已知限制

- 只提供 32 位安装包。
- 需要车机允许安装第三方应用，并允许自启动（部分车机会在熄火后清理后台）。
- 无线连接依赖手机与车机在同一 Wi-Fi 下；车机 Wi-Fi 被关闭时只能走外置蓝牙或有线。

## 许可

本项目以 [AGPL-3.0](LICENSE) 发布，基于 Display 与 XcertPlay 修改。使用时请遵守相应许可证条款。

---

## English

Free Auto CarPlay brings CarPlay to Android 4.0+ car head units. It connects to an iPhone over an external USB Bluetooth receiver, the head unit's own Bluetooth, or a USB cable — no head-unit modification and no root required.

- 32-bit (`armeabi-v7a`) builds for Android 4.0–9 head units.
- First-run wizard measures the head unit and picks the connection route for you.
- In-app OTA updates that keep settings, pairing and wizard progress.
- Steering-wheel key learning, single-file log export, crash logging.

Download the latest build from [Releases](https://github.com/Free-Auto-Car/Free-Auto-Carplay/releases).

Based on Display and XcertPlay, licensed under [AGPL-3.0](LICENSE).
