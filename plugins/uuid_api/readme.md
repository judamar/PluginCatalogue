**English** | [中文](readme-zh_cn.md)

\>\>\> [Back to index](/readme.md)

## uuid_api

### Basic Information

- Plugin ID: `uuid_api`
- Version: *Data fetching failed*
- Total downloads: N/A
- Authors: [Andy Zhang](https://github.com/AnzhiZhang)
- Repository: https://github.com/AnzhiZhang/MCDReforgedPlugins
- Repository plugin page: https://github.com/AnzhiZhang/MCDReforgedPlugins/tree/master/src/uuid_api
- Labels: [`API`](/labels/api/readme.md), [`Tool`](/labels/tool/readme.md)
- Description: *Data fetching failed*

### Dependencies

*Data fetching failed*

### Requirements

*Data fetching failed*

### Introduction

# UUID API

> Player UUID API

## Required Python Modules

- requests

## Usage

```python
get_uuid(name: str) -> UUID | None
```

Returns `None` if the player is not found.

Example:

```python
uuid_api = server.get_plugin_instance('uuid_api')
uuid = uuid_api.get_uuid('Steve')
server.logger.warning(uuid)
```

## Configuration

### use_usercache

Default: `true`

Whether to use data from the `usercache.json` file as a cache to retrieve player UUIDs.

### override_online_mode

Default: `false`

Whether to override the `online-mode` setting in `server.properties`.

If set to `true`, the plugin will ignore the `online-mode` setting in `server.properties` and instead use the value specified in `override_online_mode_value`.

If you're using a proxy server such as BungeeCord or Velocity with online-mode enabled, or if the actual UUIDs do not match the server's `online-mode` setting, enabling this option ensures the plugin correctly handles online mode.

### override_online_mode_value

Default: `true`

When `override_online_mode` is set to `true`, this value determines whether the plugin treats the server as running in online mode.

## Acknowledgements

Some code are adapted from <https://github.com/gubaiovo/MCDR_uuid_api_remake>

### Download

> [!IMPORTANT]
> Read the README file in plugin repository before using it.

*Data fetching failed*

