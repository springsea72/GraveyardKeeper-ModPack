# GraveyardKeeperAutoSaveOnExit

## 简体中文

### 功能

自动存档扩展。当前会在返回主菜单前、正常退出游戏时，以及游戏中每过一天后自动存档。

### 注意

强制结束进程、断电、任务管理器强杀等异常退出，可能绕过 Unity 的退出事件，因此不能保证触发退出存档。

### 配置文件

`BepInEx/config/local.chunhai.graveyardkeeper.autosaveonexit.cfg`

当前配置：

```ini
SaveOnEachNewDay = true
NewDaySaveDelaySeconds = 1
DelayNewDaySaveWhileSleepGui = true
SaveBeforeReturnToMainMenu = true
SaveOnApplicationQuit = true
```

## English

### Feature

Automatic save extension. It currently saves before returning to the main menu, during normal application quit, and once after each in-game day changes.

### Note

Forced process termination, power loss, or killing the game through Task Manager may bypass Unity quit events, so the quit save cannot be guaranteed in those cases.

### Configuration File

`BepInEx/config/local.chunhai.graveyardkeeper.autosaveonexit.cfg`

Current settings:

```ini
SaveOnEachNewDay = true
NewDaySaveDelaySeconds = 1
DelayNewDaySaveWhileSleepGui = true
SaveBeforeReturnToMainMenu = true
SaveOnApplicationQuit = true
```
