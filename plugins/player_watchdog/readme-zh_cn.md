[English](readme.md) | **中文**

\>\>\> [回到索引](/readme-zh_cn.md)

## player_watchdog

### 基本信息

- 插件 ID: `player_watchdog`
- 版本: *数据拉取失败*
- 总下载量: N/A
- 作者: [LinHouyu](https://github.com/LinHouYu)
- 仓库: https://github.com/LinHouYu/Watch_dog_online_players_with_coords_and_dim
- 仓库插件页: https://github.com/LinHouYu/Watch_dog_online_players_with_coords_and_dim/tree/main
- 标签: [`管理`](/labels/management/readme-zh_cn.md), [`信息`](/labels/information/readme-zh_cn.md)
- 描述: *数据拉取失败*

### 插件依赖

*数据拉取失败*

### 包依赖

*数据拉取失败*

### 介绍

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

### 下载

> [!IMPORTANT]
> 使用插件之前，先阅读仓库中的 README。

*数据拉取失败*

