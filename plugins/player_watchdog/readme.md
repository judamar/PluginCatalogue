**English** | [中文](readme-zh_cn.md)

\>\>\> [Back to index](/readme.md)

## player_watchdog

### Basic Information

- Plugin ID: `player_watchdog`
- Version: *Data fetching failed*
- Total downloads: N/A
- Authors: [LinHouyu](https://github.com/LinHouYu)
- Repository: https://github.com/LinHouYu/Watch_dog_online_players_with_coords_and_dim
- Repository plugin page: https://github.com/LinHouYu/Watch_dog_online_players_with_coords_and_dim/tree/main
- Labels: [`Management`](/labels/management/readme.md), [`Information`](/labels/information/readme.md)
- Description: *Data fetching failed*

### Dependencies

*Data fetching failed*

### Requirements

*Data fetching failed*

### Introduction

# Player Watchdog

一个基于 [MCDReforged](https://mcdreforged.com/) 的插件，用于定时记录在线玩家的坐标、维度和物品信息，并保存为 CSV 文件，方便用 Excel 查看和分析。

## 功能特性
- **自动记录在线玩家信息**  
  每隔固定时间（默认 5 秒）获取所有在线玩家的：
  - 坐标（X, Y, Z）
  - 所在维度（主世界 / 地狱 / 末地）
  - 物品栏（Inventory）
- **CSV 格式输出**
  - 文件体积小，长期保存无压力
  - 可直接用 Excel 打开，支持筛选、排序、统计
  - 字段：时间、玩家、维度、X、Y、Z、物品
  - <img width="1620" height="393" alt="image" src="https://github.com/user-attachments/assets/10fd545f-f901-4d63-9106-b265f3822aba" />

## 使用方法
1. 将本插件文件夹放入 `plugins/` 目录
2. 确保已安装并启用 [Minecraft Data API](https://mcdreforged.com/zh-CN/plugin/minecraft_data_api) 插件
3. 在 MCDR 的 Python 环境中安装依赖：
   ```bash
   pip install hjson
   ```

### Download

> [!IMPORTANT]
> Read the README file in plugin repository before using it.

*Data fetching failed*

