# Macro Shelf-A 0.9.6.3 发布说明

在国服卫月插件安装器刷新自定义仓库后，更新 **Macro Shelf-A**。输入 `/aklmacro version` 可确认实际加载的版本为 **0.9.6.3**。[在线仓库](https://github.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/tree/main/plugins/MacroShelfA)

- 从剪贴板追加或替换宏时，写盘成功后才切换资料库。新增、复制、移动或删除宏遇到保存错误，也会恢复原顺序和倒计时绑定，允许重试。
- 启动时修复缺失或重复的宏 ID。遇到两个条目共用同一个 ID，原游戏热键入口会停止运行。请在“生成游戏热键入口”中选择正确条目并重新生成。
- 宏名称和分类在长度上限处保留完整的表情字符。升级配置时，插件先写出完整备份；遇到损坏的备份或更高版本的配置会停止加载并提示原因。
- 修复加载中断时遗留事件订阅的问题。执行器或等待设置在保存成功后才生效。

本版面向国服 Dalamud API 15 和 Windows x64。离线验证通过 386 项逻辑、接口及加载检查和 4,877 条 ImGui 界面断言。游戏内热键跨重登、等待补丁恢复以及卸载期间取消原生宏仍待实测。[历史版本与本版校验资料](https://github.com/Alittlerecallinglittlebrother/DalamudCN-Plugins/tree/main/plugins/MacroShelfA)

对应维护提交为 `3677383297f4cded235748b4054411c1f6568971`。[源码提交](https://github.com/Alittlerecallinglittlebrother/MacroShelfA/commit/3677383297f4cded235748b4054411c1f6568971) · [本次构建与测试](https://github.com/Alittlerecallinglittlebrother/MacroShelfA/actions/runs/42322170120)
