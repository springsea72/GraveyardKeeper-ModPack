# Graveyard Keeper BepInEx Mod Pack

## 简体中文

这是一个已经整理好的 Graveyard Keeper Windows 版 BepInEx mod 发布包。包内结构按游戏根目录准备，包含 BepInEx、Doorstop 启动文件、所有已制作的 mod DLL，以及当前正在使用的配置文件。

### 安装方法

1. 完全退出游戏。
2. 打开游戏根目录，也就是 `Graveyard Keeper.exe` 所在目录。
3. 将本发布文件夹内的所有内容复制到游戏根目录中。
4. 如果系统提示合并 `BepInEx` 文件夹或覆盖同名文件，选择合并/覆盖。
5. 启动游戏。
6. 如需确认加载情况，可查看 `BepInEx/LogOutput.log`。

注意：不要只把整个发布文件夹作为一个子文件夹放进游戏目录。必须复制本文件夹里面的 `BepInEx`、`winhttp.dll`、`doorstop_config.ini` 到 `Graveyard Keeper.exe` 同级目录。

### 包含的文件

- `winhttp.dll`：BepInEx/Doorstop 启动入口。
- `doorstop_config.ini`：Doorstop 配置。
- `BepInEx/core`：BepInEx 核心运行库。
- `BepInEx/plugins`：mod DLL。
- `BepInEx/config`：当前默认配置。

### 包含的 mod 与当前默认配置

| Mod | 功能 | 当前默认配置 |
| --- | --- | --- |
| GraveyardKeeperInventoryExpander | 扩展玩家主物品栏 | `TargetSlots = 400` |
| GraveyardKeeperToolDurabilityGuard | 斧头、十字镐、铁铲不损失耐久 | `ProtectAxes = true`, `ProtectPickaxes = true`, `ProtectShovels = true` |
| GraveyardKeeperInfiniteEnergy | 无限能量/精力 | `KeepEnergyFull = true`, `PreventEnergyDecrease = true`, `SkipSpendChecks = true` |
| GraveyardKeeperAutoSaveOnExit | 退出游戏和每日自动存档 | `SaveBeforeReturnToMainMenu = true`, `SaveOnApplicationQuit = true`, `SaveOnEachNewDay = true`, `NewDaySaveDelaySeconds = 1` |
| GraveyardKeeperAutoRegen | 非睡觉期间自动回血 | `EnableAutoRegen = true`, `SleepRateMultiplier = 0.2`, `RegenWhilePaused = false`, `RegenDuringSleepGui = false` |
| GraveyardKeeperFastMovement | 玩家移动速度提升 | `EnableFastMovement = true`, `SpeedMultiplier = 1.5`, `StackWithSpeedPotion = true` |
| GraveyardKeeperNoMortuaryWait | 防腐台注射和远程解剖台操作立即完成 | `InstantEmbalmingTable = true`, `InstantRemoteAutopsyTable = true` |
| GraveyardKeeperTeleportStoneTweaks | 传送石无冷却并绑定快捷键 | `CooldownSeconds = 0`, `EnableHotkey = true`, `Hotkey = F9` |

### 配置文件位置

所有 mod 配置都在 `BepInEx/config` 下。修改配置后，重启游戏生效。

本发布包已排除旧测试 mod 配置 `local.chunhai.graveyardkeeper.testmod.cfg`。

### 卸载方法

删除 `BepInEx/plugins` 下对应 mod 文件夹或 DLL 即可禁用单个 mod。若要完全移除 BepInEx，请删除 `BepInEx` 文件夹、`winhttp.dll` 和 `doorstop_config.ini`。

## English

This is a prepared BepInEx mod release package for the Windows version of Graveyard Keeper. The package is laid out like the game root directory and includes BepInEx, Doorstop bootstrap files, all created mod DLLs, and the currently used configuration files.

### Installation

1. Close the game completely.
2. Open the game root directory, the folder that contains `Graveyard Keeper.exe`.
3. Copy all contents inside this release folder into the game root directory.
4. If Windows asks to merge the `BepInEx` folder or overwrite files, choose merge/overwrite.
5. Start the game.
6. To confirm loading, check `BepInEx/LogOutput.log`.

Important: Do not place this whole release folder as a nested subfolder inside the game directory. You must copy the contents inside it, including `BepInEx`, `winhttp.dll`, and `doorstop_config.ini`, next to `Graveyard Keeper.exe`.

### Included Files

- `winhttp.dll`: BepInEx/Doorstop bootstrap entry.
- `doorstop_config.ini`: Doorstop configuration.
- `BepInEx/core`: BepInEx runtime libraries.
- `BepInEx/plugins`: mod DLLs.
- `BepInEx/config`: current default configuration files.

### Included Mods and Current Defaults

| Mod | Feature | Current defaults |
| --- | --- | --- |
| GraveyardKeeperInventoryExpander | Expands the player main inventory | `TargetSlots = 400` |
| GraveyardKeeperToolDurabilityGuard | Prevents durability loss for axes, pickaxes, and shovels | `ProtectAxes = true`, `ProtectPickaxes = true`, `ProtectShovels = true` |
| GraveyardKeeperInfiniteEnergy | Infinite player energy/stamina | `KeepEnergyFull = true`, `PreventEnergyDecrease = true`, `SkipSpendChecks = true` |
| GraveyardKeeperAutoSaveOnExit | Saves on exit and once per in-game day | `SaveBeforeReturnToMainMenu = true`, `SaveOnApplicationQuit = true`, `SaveOnEachNewDay = true`, `NewDaySaveDelaySeconds = 1` |
| GraveyardKeeperAutoRegen | Regenerates HP outside sleeping | `EnableAutoRegen = true`, `SleepRateMultiplier = 0.2`, `RegenWhilePaused = false`, `RegenDuringSleepGui = false` |
| GraveyardKeeperFastMovement | Increases player movement speed | `EnableFastMovement = true`, `SpeedMultiplier = 1.5`, `StackWithSpeedPotion = true` |
| GraveyardKeeperNoMortuaryWait | Instantly finishes embalming-table injections and remote autopsy-table operations | `InstantEmbalmingTable = true`, `InstantRemoteAutopsyTable = true` |
| GraveyardKeeperTeleportStoneTweaks | Removes teleport stone cooldown and adds a hotkey | `CooldownSeconds = 0`, `EnableHotkey = true`, `Hotkey = F9` |

### Configuration Files

All mod configuration files are in `BepInEx/config`. Restart the game after editing them.

The old test mod configuration `local.chunhai.graveyardkeeper.testmod.cfg` has been excluded from this release package.

### Uninstall

To disable a single mod, delete its folder or DLL under `BepInEx/plugins`. To remove BepInEx completely, delete the `BepInEx` folder, `winhttp.dll`, and `doorstop_config.ini`.
