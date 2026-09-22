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

版本 **0.8.4.0**，卫月 API 15，作者：Akl。简介：**当我受够了FF14那糟糕的宏指令**。

数字切装后的公共执行流程现会等待职业与目标套装同步，再继续聊天、表情、中文动作、技能、独立等待及下一次切装；主窗口和常用栏显示等待原因。原生命令入口采用 ProcessChatBoxEntry，可选动作诊断默认关闭。保留 A+B 界面、独立常用宏栏、用户原图、零额外行间隔、宏组、长宏、小数等待和倒计时触发。

**已知的表情绕过切职保护、在旧职业状态提前派发的代码缺口已修正；职业与套装状态一致不等于动画或技能已就绪，不增加固定延迟或动作重试。

[使用说明、插件包与对应源码](plugins/MacroShelfA/README.md)

版本 `3.2.5.11`，卫月 API 15。作者：akira0245, Ori, Kalle, Zune, 断水剑。

本版加入按角色名与原属服务器匹配的本机欢迎语音，支持独立音量、试听和停止，并修复欢迎模块在卫月内存加载 DLL 时导致整个插件加载失败的问题。保留记录删除、清理及未归档演出 JSON/CSV 导出功能。

## 点数统计（点数比拼）

版本 **1.1.0.0**，卫月 API 15，作者：断水剑。使用 `/dstat` 打开。

独立统计 `/random` 的最高、最低或最接近目标数字的玩家；开始自动公告，结束按所选规则公布全部并列第一。公告文字、目标数字和发送频道均可自行设置，默认呼喊 `/shout`。保留逐次记录、归档、复制排名及 CSV 导出。

[安装说明、插件包与对应源码](plugins/DiceStats/README.md)
