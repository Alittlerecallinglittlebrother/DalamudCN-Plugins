# 插件收纳盒（PluginShelf）

当前在线版本 **0.1.2.0**。Dalamud API 15 / .NET 10 / Windows x64。

把已安装插件的标准界面入口收纳为小型快捷栏：置顶入口直接点击，其余在可搜索的折叠收藏夹中打开。支持主界面与设置分别收藏、中文别名、拖动排序；不会安装、启停或修改其他插件。

## 在线安装

在 DalamudCN 设置的「自定义插件仓库」添加下列地址；已经添加过的用户只需刷新插件列表：

```text
https://raw.githubusercontent.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/main/repo.json
```

搜索 **插件收纳盒** 后安装。此前使用过同名本地开发插件的，请先停用本地版，避免同时加载；原来的 `shelf.json` 不需要删除。首次进入在「全部插件」收藏常用入口。右键快捷栏的「收纳」可解锁并移动位置；可用 `/pluginshelf reset` 找回。

[插件包](0.1.2.0/PluginShelf.zip) · [对应源码](0.1.2.0/PluginShelf-source.zip) · [发布说明](0.1.2.0/RELEASE.md) · [校验值](0.1.2.0/SHA256SUMS.txt)

[快捷栏离线预览](0.1.2.0/dock-offline.png) · [收藏夹离线预览](0.1.2.0/tray-offline.png)

## 验证边界

Release 构建零错误、零警告；核心 30 项、后端 20 项、原生 ImGui UI 52 项离线测试通过。预览图使用合成插件目录，并非游戏截图。**v0.1.2.0 未在游戏内加载、未逐一验证第三方插件窗口**，请自行确认游戏内操作与不同字体、分辨率的表现。发行时没有触碰用户现有游戏配置。
