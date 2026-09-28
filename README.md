# DalamudCN Plugins

用于集中安装以下 DalamudCN 插件的在线仓库：

- `LiveFakeName`
- `Macro Shelf-A`
- `Nearby Player List`
- `Auto Face`
- `Auto Gail`
- `FuckFurniture`
- `Slidecasting goat`
- `midibard2-深海回响特供版`
- `点数统计`

## 在线安装

在 DalamudCN 设置的“自定义插件仓库”中添加：

```text
https://raw.githubusercontent.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/main/repo.json
```

保存后即可在插件安装器中搜索并安装上述插件。

插件安装包、图标和版本信息由本仓库或对应插件仓库提供。

## Macro Shelf-A

版本 **0.9.5.2**，卫月 API 15，作者：Akl。简介：**当我受够了FF14那糟糕的宏指令**。

**原生宏执行默认开启**，不需要时可手动关闭并记住选择。新配置及缺失该字段的旧配置采用开启；已有保存为关闭的配置不强制覆盖。备份缺省值同步调整，追加导入不改变当前设置。

原生 ExecuteMacro、长宏分段和等待机制不变；保留旧逐行模式、三主题、原图和宏正文。开关文案仍为“原生宏执行”，说明仅“整段交给游戏执行。”。2922 项离线检查通过，Release 构建零错误、零警告。

原生路径仍仅支持已审计客户端，保留已知 CancelMacro Byte/Void 绑定校验提示。Runtime 与已有舞蹈实测的 0.9.5.0 不变；新 DLL 未另做完整游戏验收。

[使用说明、已知问题、插件包与对应源码](plugins/MacroShelfA/README.md)

## midibard2-深海回响特供版

版本 `3.2.5.11`，卫月 API 15。作者：akira0245, Ori, Kalle, Zune, 断水剑。

观众聊天点歌自动排队，支持单人和合奏主控。演出房间支持队伍外主持人与队长共同管理队列，以及最多七名队员只读查看当前曲目、下一首和待演顺序，共用樱花 TCP 隧道。安装前停用原版或旧版 MidiBard2 开发插件，避免相同内部标识重复加载。实际公网连接、游戏内演奏和多人合奏仍待验证。

本版加入按角色名与原属服务器匹配的本机欢迎语音，支持独立音量、试听和停止，并修复欢迎模块在卫月内存加载 DLL 时导致整个插件加载失败的问题。保留记录删除、清理及未归档演出 JSON/CSV 导出功能。232 项核心测试及实际 DLL 内存加载、原音频播放检查通过；游戏内加载和欢迎触发仍待验收。

[使用说明与对应源码](plugins/MidiBard2/README.md)

## 点数统计（点数比拼）

版本 **1.1.0.0**，卫月 API 15，作者：断水剑。使用 `/dstat` 打开。

独立统计 `/random` 的最高、最低或最接近目标数字的玩家；开始自动公告，结束按所选规则公布全部并列第一。公告文字、目标数字和发送频道均可自行设置，默认呼喊 `/shout`。保留逐次记录、归档、复制排名及 CSV 导出。

28 项核心测试、74 项流程/队列/原生界面检查通过；真实游戏内加载及公告收发尚待验收。

[安装说明、插件包与对应源码](plugins/DiceStats/README.md)
