# 来源与第三方组件

插件署名：Aida Enna、断水剑。Aida Enna 是原版 Doorbell 作者，断水剑是本地修改版新增署名；此署名不表示原作者参与或认可本地修改。

## 功能参考

本项目基于对 Aida Enna 的 Doorbell 项目功能和行为的研究，面向本地国服使用重新组织实现：

https://github.com/Aida-Enna/Doorbell

参考时的提交：4ca64ffa6ffe37115740700ba79ddd4cc97ff004。

原仓库未发现明示的 LICENSE 文件，不应将“公开可见”误当成自动取得任意复制和再分发授权。本地重构使用独立插件标识 DoorbellCN；不代表原作者、国服启动器团队或 Square Enix 官方版本。没有复制原仓库的图标或提示音；本包的提示音由 tools/generate_chime.py 合成。

如计划公开发布而不只是本地使用，应另行审查原项目、Dalamud、FFXIVClientStructs 及相关依赖的授权与游戏规则；本说明不替代授权或法律意见。

## 随包分发的组件

- NAudio.Core 2.2.1
- NAudio.WinMM 2.2.1
- NAudio.Wasapi 2.2.1

项目：https://github.com/naudio/NAudio

以上组件遵循 MIT 授权，完整声明保留于 licenses/NAudio-LICENSE.txt。

Dalamud、FFXIVClientStructs、Lumina 和 ImGui 等由用户的国服 Dalamud 环境提供，本交付包不包含或替换这些宿主 DLL。
