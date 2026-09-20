# DalamudCN Plugins

用于集中安装以下 DalamudCN 插件的在线仓库：

- `LiveFakeName`
- `Macro Shelf-A`
- `Nearby Player List`
- `Auto Face`
- `Auto Gail`
- `FuckFurniture`
- `Slidecasting goat`

## 在线安装

在 DalamudCN 设置的“自定义插件仓库”中添加：

```text
https://raw.githubusercontent.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/main/repo.json
```

保存后即可在插件安装器中搜索并安装上述插件。

插件安装包、图标和版本信息由本仓库或对应插件仓库提供。

## Macro Shelf-A

版本 `0.4.1.0`，卫月 API 15，作者：Akl。支持自定义总宏按钮、子宏分类与顺序衔接、单独运行子宏，以及默认关闭的“解除 15 行限制”开关。开启后独立宏和子宏均可超过 15 行，每宏支持 64,000 字符；保留等待、整组中止和悬浮入口。

45 项自动化检查与原生 ImGui 交互测试通过，游戏内效果尚未实测。

[使用说明、插件包与对应源码](plugins/MacroShelfA/README.md)

版本 `3.2.5.11`，卫月 API 15。作者：akira0245, Ori, Kalle, Zune, 断水剑。

本版加入按角色名与原属服务器匹配的本机欢迎语音，支持独立音量、试听和停止，并修复欢迎模块在卫月内存加载 DLL 时导致整个插件加载失败的问题。保留记录删除、清理及未归档演出 JSON/CSV 导出功能。
