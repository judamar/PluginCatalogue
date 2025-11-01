**English** | [中文](readme-zh_cn.md)

\>\>\> [Back to index](/readme.md)

## simple_tp

### Basic Information

- Plugin ID: `simple_tp`
- Version: *Data fetching failed*
- Total downloads: N/A
- Authors: [PairZhu](https://github.com/PairZhu)
- Repository: https://github.com/PairZhu/SimpleTP-MCDR
- Repository plugin page: https://github.com/PairZhu/SimpleTP-MCDR/tree/master
- Labels: [`Tool`](/labels/tool/readme.md)
- Description: *Data fetching failed*

### Dependencies

*Data fetching failed*

### Requirements

*Data fetching failed*

### Introduction

# SimpleTP
**English** | [简体中文](https://github.com/PairZhu/SimpleTP-MCDR/tree/master/README.zh.md)

A simple teleportation plugin designed to create waypoints and implement the teleportation features of EssentialsX.

## Preview
![help](https://raw.githubusercontent.com/PairZhu/SimpleTP-MCDR/master/image/README/1757133291389.png)
![list](https://raw.githubusercontent.com/PairZhu/SimpleTP-MCDR/master/image/README/1757133317304.png)
![back](https://raw.githubusercontent.com/PairZhu/SimpleTP-MCDR/master/image/README/1757133375310.png)

## Features
- Support for personal waypoints that players can create and manage, visible only to themselves
- Support for global waypoints (public waypoints) visible to all players, suitable for public areas
- Configurable enabled dimensions with support for modded dimensions (like Twilight Forest, Eternal Starlight, etc.)
- Support for returning to death location and previous location before teleporting
- Most commands support clickable operations for convenience
- Easytp syntax sugar: `stp xxx` is equivalent to `stp tpp/tpg/tp/tpa xxx`, automatically recognizing waypoints and players, with priority `Personal Waypoint > Global Waypoint > Player`
- Support for comprehensive command argument completion, allowing the use of the Tab key to complete waypoint names and player names (requires the [command_suggest](https://mcdreforged.com/en/plugin/command_suggest) plugin)

## Commands
The following examples use the default prefix "!!stp". Adjust according to your configuration file.
- !!stp help View help information

Preview commands can be found in the [language file](https://github.com/PairZhu/SimpleTP-MCDR/tree/master/./lang/en_us.yml) under the help section.

## Configuration File
The configuration file is located at `config/SimpleTP/config.json`
- **prefix**: Command prefix, default is `!!stp`
- **back_on_death**: Whether to automatically record the position upon player death, default is `true`
- **save_interval**: Interval for scheduled saving of waypoint data, in seconds, default is `30` seconds
- **permissions**: Permission configuration
- **worlds**: List of supported dimensions (including mod dimensions), default is `["minecraft:overworld", "minecraft:the_nether", "minecraft:the_end"]`. Teleportation will not work in dimensions not in this list. To disable teleportation in a dimension, simply remove it from the list.
- **extra_dimensions**: ***Only required for Minecraft versions before 1.16***, configuration format is `{<dimension_id>: "<dimension_name>"}`, for example `{0: "minecraft:overworld", 1: "minecraft:the_nether", 2: "minecraft:the_end"}`. This configuration is used to support mod dimensions in older Minecraft versions.
- **easy_tp**: Whether to enable easytp syntax sugar, default is `true`.

### Permission Configuration
- **back**: Permission to use `!!stp back` command
- **tpa**: Permission to use `!!stp tpa` command
- **tpahere**: Permission to use `!!stp tpahere` command
- **tp**: Permission to use `!!stp tp <player>` command
- **tphere**: Permission to use `!!stp tphere <player>` command
- **personal_waypoint**: Permission to set/delete personal waypoint related commands
- **global_waypoint**: Permission to set/delete global waypoint related commands
- **cross_world_tp**: Permission for cross-dimension teleportation

## Dependencies
- **minecraft_data_api**: Used for retrieving player information
- **mg_events**: Used for listening to player death events

## Common Issues
- **Clickable Teleport Button Not Responding**
  MCDR has issues with click execution support in higher MC versions. Install [LetMeClickAndSendForServer](https://github.com/Fallen-Breath/LetMeClickAndSendForServer) (server-side) or [LetMeClickAndSend](https://github.com/Fallen-Breath/LetMeClickAndSend) (client-side).
- **Sometimes `back` Command Doesn't Return to Previous Location After Death**
  Some mod death messages are special and may not be detected by mg_events. You need to manually add corresponding death messages in mg_events language files. For example, for the [Eternal Starlight](https://www.curseforge.com/minecraft/mc-mods/eternal-starlight) mod, when players die in the Ether, add `"death.attack.ether": "%1$s drifts away"` to `config/mg_events/lang/en_us.json`, and `"death.attack.ether": "%1$s飘然而去"` to `config/mg_events/lang/zh_cn.json`.
- **Log Shows "Player {player} is in a dimension not enabled in config: {dimension}"**
  This indicates the player is in a dimension not enabled in the configuration. Check the `worlds` configuration in `config/SimpleTP/config.json` to ensure the dimension is included.
- **Log Shows "Player {player} is in an unknown dimension with ID {dimension}"**
  This error may occur when the server Minecraft version is before 1.16 and mod dimensions are installed. Check the `extra_dimensions` configuration in `config/SimpleTP/config.json` to ensure the dimension is included. You can get the dimension ID using the `/data get entity <player> Dimension` command.

## TODO
If you have more feature requests or are interested in any planned features, feel free to raise them in the issues section 🚀
Sorted by priority:
- [x] Support clickable waypoints
- [x] `back` command supports round-trip teleportation
- [x] Record player's dimension in waypoints (Nether, Overworld, End)
- [x] Configuration for cross-dimension teleportation
- [x] Scheduled saving of waypoint data (to prevent loss on crash)
- [x] `tp`/`tphere` functionality
- [x] `tpa`/`tpahere` functionality
- [x] Multi-language support
- [x] Help information
- [ ] Record player's orientation in waypoints
- [ ] Add description information for waypoints
- [ ] Teleport cooldown configuration
- [ ] Maximum number of waypoints configuration
- [ ] Waypoint name length limit configuration
- [ ] Waypoint safety check, prompting confirmation or teleporting to nearby safe location if the waypoint is in a dangerous position
- [ ] Teleport cost configuration (consume custom items or experience) (base cost + distance cost)

### Download

> [!IMPORTANT]
> Read the README file in plugin repository before using it.

*Data fetching failed*

