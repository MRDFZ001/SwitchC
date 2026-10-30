# 固件源码

源码文件：`SwitchC_S2_v0.2.0.ino`（版本 0.2.0）

- 板型：ESP32-S2 mini（Arduino 构建目标 `esp32.esp32.lolin_s2_mini`），仅支持这一款主板
- 核心：USB HID 模拟 Switch Pro 手柄、WiFi 配置页、板子网页后台（192.168.4.1）
- 热点：配置热点 `SwitchC-WiFi配置`（开放），工作热点 `SwitchC`（密码 12345678，教程里已公开）
- 绘图：画笔 1x1 / 3x3 / 5x5、绘图模式 smart / fast / slow / splatoon、颜色校准、安全暂停、保存数据、原点继续
- 在线：OTA 查 `switchc.shop/firmware/version.json`、分享 / 投稿走 `switchc.shop/api` 代理
- 构建产物（不进仓库）：`.elf`、`.map` 已排除；烧录用 4 个 bin 见 flash/README.md，bootloader 与网站 0.2.0 的 MD5 一致

支持游戏：朋友收集梦想生活、喷喷 3（Splatoon 3）。

许可证：GPLv3。
