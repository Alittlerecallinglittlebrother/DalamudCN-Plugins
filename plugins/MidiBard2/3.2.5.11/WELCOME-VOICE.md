# 开场欢迎语音

版本：3.2.5.11 / v0.10.1。使用用户制作的三段原始 WAV，未重新合成、变声、转码或添加音效。

本次修复 3.2.5.10 的插件加载失败：卫月通过内存载入 DLL 时 `Assembly.Location` 为空，现使用 `IDalamudPluginInterface.AssemblyLocation` 定位音频。欢迎模块初始化失败时记录错误，其他插件功能仍可启动。

| 身份（角色名@原属服务器） | 原始文件 | 插件音频资源 |
| --- | --- | --- |
| 七猫猫猫猫@伊修加德 | 七猫.wav | Assets/Welcome/qimao.wav |
| 悼亡录@红茶川 | 悼亡录.wav | Assets/Welcome/daowanglu.wav |
| 其他角色 | 其他.wav | Assets/Welcome/general.wav |

身份匹配使用完整角色名和原属服务器 HomeWorld。跨服访问不影响匹配；同名但不同原属服务器的角色使用通用语音。

## 使用

启用插件后，登录角色并首次打开 MidiBard 主界面、自动点歌界面或设置界面时，自动播放对应语音。三个入口共用一次播放限制，反复开关窗口不会重复播放。退出角色后重新登录会重新欢迎；重载插件也会重新开始一次欢迎周期。

设置窗口的“欢迎语音”页提供开关、音量、音频选择、试听和停止。默认开启、音量 55%。音量只作用于欢迎语音，不改变游戏或系统音量；多开设置同步保留各客户端自己的欢迎开关与音量。

进入乐器演奏模式、MidiBard 播放、合奏准备或自动队列正在准备歌曲时，不播放欢迎语音。欢迎播放过程中进入这些状态会立即停止，不会在歌曲间隙补播。关闭所有插件窗口、登出、静音或停用插件也会停止欢迎语音。

欢迎语音仅在本机播放，不通过游戏聊天或演出房间发送给其他玩家；不需要额外网络服务。

## 在线安装

在卫月插件安装器中刷新现有自定义仓库，安装或更新 `midibard2-深海回响特供版` 到 `3.2.5.11`。在线版与本地开发版沿用同一 `MidiBard2` 内部标识，启用在线版前请停用开发插件入口。安装器会一同安装三段欢迎音频和播放依赖。

## 开发插件

先停用在线版或旧开发版，再把下列 DLL 加到卫月开发插件列表并启用：

```text
%APPDATA%/XIVLauncherCN/devPlugins/MidiBard2-Deepsea-v0.10.1/MidiBard2.dll
```

`Assets/Welcome`、`NAudio.Core.dll`、`NAudio.WinMM.dll` 必须与主插件一同保留。开发脚本和安装包已包含这些资源。本版保留旧版本目录，未替换游戏中正在运行的插件。

本机原 `MidiBard2-Deepsea-v0.10` 目录经过备份后也会安装本修复版，原入口可以继续使用。确认显示 `3.2.5.11`，不要重复启用多个 MidiBard2 开发入口。

## 原始音频校验

三个文件均为 24 kHz、16-bit PCM、单声道。时长分别约 5.97 秒、6.07 秒、4.47 秒。SHA256：

```text
DE4DBD4112F5B4063A1A7CF7A44D3CC0F19B36CBE4E2B432F83600CE9CBCF34E  general.wav
D7C815E89035EAA45C63999DC9497A6DF1A8E4ECD70F45A0D09554969176D04E  qimao.wav
6A4DE6E2BBE3350408FE451856C50AA1FC0750EB0C42C48B88766E53399E73A3  daowanglu.wav
```

原录音由项目所有者提供。NAudio 用于本机播放，许可见 `STAGE-THIRD-PARTY-NOTICES.txt`（源码中为 `Stage/THIRD-PARTY-NOTICES.txt`）。验证范围见 `STAGE-VERIFICATION.md`。
