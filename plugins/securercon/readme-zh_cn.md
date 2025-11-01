[English](readme.md) | **中文**

\>\>\> [回到索引](/readme-zh_cn.md)

## securercon

### 基本信息

- 插件 ID: `securercon`
- 版本: *数据拉取失败*
- 总下载量: N/A
- 作者: [wangyupu](https://github.com/wang-yupu)
- 仓库: https://github.com/wang-yupu/SecureRCON
- 仓库插件页: https://github.com/wang-yupu/SecureRCON/tree/main
- 标签: [`管理`](/labels/management/readme-zh_cn.md)
- 描述: *数据拉取失败*

### 插件依赖

*数据拉取失败*

### 包依赖

*数据拉取失败*

### 介绍


# SecureRCON

一个MCDR插件，加密你的RCON访问，扩展RCON功能

## Why?

原版的RCON是明文传输的（包括密钥与内容），因此加密RCON是有用的。扩展RCON后，可以执行MCDR指令和聊天。

## 加密方法和访问方法

此MCDR插件安装后会作为原始RCON的一个*代理*，替代鉴权部分，同时提供加密支持。  
安装此插件后，如果机器的任意端口都暴露到网络，请使用防火墙进行拦截(e.g. ufw / firewalled / iptables)，同时设定一个较强的RCON密码。本插件会自动读取RCON密码，并监听一个端口(默认25576)，此端口的协议兼容原始RCON，若依然使用原版RCON客户端，可以使用固定强密码或者动态密码。

### SecureMCRCON Python Package

> 执行 `pip install securemcrcon` 以安装，然后使用`smcrcon`命令  
> [Repo](https://github.com/wang-yupu/SecureMCRCON)  
> [PyPI](https://pypi.org/project/securemcrcon/)

CLI客户端

### MCRCON App

> Coming soon (第二优先级)

<!-- [GitHub](https://github.com/wang-yupu/)
此应用支持Windows / macOS(Coming Soon) / Linux(Coming Soon) / Android，可以用此应用进行加密RCON连接，本身也是一个不错的RCON图形化客户端 -->

### 下载

> [!IMPORTANT]
> 使用插件之前，先阅读仓库中的 README。

*数据拉取失败*

