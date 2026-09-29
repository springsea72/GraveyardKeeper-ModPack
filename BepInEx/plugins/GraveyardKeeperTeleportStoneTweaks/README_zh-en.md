# GraveyardKeeperTeleportStoneTweaks

## 简体中文

### 功能

调整传送石：

- 传送石冷却时间为 `0` 秒。
- 默认快捷键为 `F9`。
- 按快捷键会从玩家背包中查找传送石并调用原版使用逻辑，因此仍会打开原版传送地点选择界面。

### 配置文件

`BepInEx/config/local.chunhai.graveyardkeeper.teleportstonetweaks.cfg`

当前配置：

```ini
EnableCooldownTweaks = true
CooldownSeconds = 0
EnableHotkey = true
Hotkey = F9
LogMissingStone = false
```

## English

### Feature

Tweaks the teleport stone:

- Teleport stone cooldown is `0` seconds.
- The default hotkey is `F9`.
- Pressing the hotkey searches the player's inventory for the teleport stone and calls the original use logic, so the original destination selection UI is still used.

### Configuration File

`BepInEx/config/local.chunhai.graveyardkeeper.teleportstonetweaks.cfg`

Current settings:

```ini
EnableCooldownTweaks = true
CooldownSeconds = 0
EnableHotkey = true
Hotkey = F9
LogMissingStone = false
```
