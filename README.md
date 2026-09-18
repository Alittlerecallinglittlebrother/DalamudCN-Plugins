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

## 在线安装

在 DalamudCN 设置的“自定义插件仓库”中添加：

```text
https://raw.githubusercontent.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/main/repo.json
```

保存后即可在插件安装器中搜索并安装上述插件。

插件安装包、图标和版本信息由本仓库或对应插件仓库提供。

## midibard2-深海回响特供版

版本 `3.2.5.9`，卫月 API 15。作者：akira0245, Ori, Kalle, Zune, 断水剑。

观众聊天点歌自动排队，支持单人和合奏主控。演出房间支持队伍外主持人与队长共同管理队列，以及最多七名队员只读查看当前曲目、下一首和待演顺序，共用樱花 TCP 隧道。安装前停用原版或旧版 MidiBard2 开发插件，避免相同内部标识重复加载。实际公网连接、游戏内演奏和多人合奏仍待验证。

本版为已结束列表、节目单、点歌记录及演出记录添加删除和清理按钮；未归档演出也可直接导出 JSON/CSV，并打开导出文件夹。

[使用说明与对应源码](plugins/MidiBard2/README.md)
