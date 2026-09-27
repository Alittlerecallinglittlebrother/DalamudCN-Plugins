# DalamudCN Plugins

用于集中安装以下 DalamudCN 插件的在线仓库：

- `LiveFakeName`
- `Macro Shelf-A`
- `Nearby Player List`
- `Auto Face`
- `Auto Gail`
- `FuckFurniture`
- `Slidecasting goat`
- `点数统计`

## 在线安装

在 DalamudCN 设置的“自定义插件仓库”中添加：

```text
https://raw.githubusercontent.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/main/repo.json
```

保存后即可在插件安装器中搜索并安装上述插件。

插件安装包、图标和版本信息由本仓库或对应插件仓库提供。

## Macro Shelf-A

版本 **0.9.5.1**，卫月 API 15，作者：Akl。简介：**当我受够了FF14那糟糕的宏指令**。

新增原生 ExecuteMacro 与长宏分段续接；保留原文等待、旧逐行执行、三主题、原图和既有宏数据。一份69行舞蹈实测恢复占星后蹦跳，两轮五段完整运行。0.9.5.1 将开关名精简为“原生宏执行”，下方只留“整段交给游戏执行。”，Runtime与实测0.9.5.0不变；

**原生模式默认关闭**，需在设置启用或输入 `/aklmacro engine native`，仅支持已审计客户端。保留已知 CancelMacro Byte/Void 绑定校验提示；外部取消/接管未全面实测。

[使用说明、已知问题、插件包与对应源码](plugins/MacroShelfA/README.md)

版本 `3.2.5.11`，卫月 API 15。作者：akira0245, Ori, Kalle, Zune, 断水剑。

本版加入按角色名与原属服务器匹配的本机欢迎语音，支持独立音量、试听和停止，并修复欢迎模块在卫月内存加载 DLL 时导致整个插件加载失败的问题。保留记录删除、清理及未归档演出 JSON/CSV 导出功能。

## 点数统计（点数比拼）

版本 **1.1.0.0**，卫月 API 15，作者：断水剑。使用 `/dstat` 打开。

独立统计 `/random` 的最高、最低或最接近目标数字的玩家；开始自动公告，结束按所选规则公布全部并列第一。公告文字、目标数字和发送频道均可自行设置，默认呼喊 `/shout`。保留逐次记录、归档、复制排名及 CSV 导出。

[安装说明、插件包与对应源码](plugins/DiceStats/README.md)
