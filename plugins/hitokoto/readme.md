**English** | [中文](readme-zh_cn.md)

\>\>\> [Back to index](/readme.md)

## hitokoto

### Basic Information

- Plugin ID: `hitokoto`
- Version: *Data fetching failed*
- Total downloads: N/A
- Authors: [gubai](https://github.com/gubaiovo)
- Repository: https://github.com/gubaiovo/MCDR_hitokoto
- Repository plugin page: https://github.com/gubaiovo/MCDR_hitokoto/tree/main/hitokoto
- Labels: [`API`](/labels/api/readme.md), [`Tool`](/labels/tool/readme.md)
- Description: *Data fetching failed*

### Dependencies

*Data fetching failed*

### Requirements

*Data fetching failed*

### Introduction

# MCDR Hitokoto
Call the [Hitokoto](https://hitokoto.cn/) API and automatically output the result to the server.

### Configuration File

```json
{
    "interval": "10s",
    "parameters": {},
    "base_url": "https://v1.hitokoto.cn/",
    "from_where": true
}
```

- `interval` : Fetch interval. Supported units: `s`, `m`, `h`. Minimum value is `10s`.
- `base_url` : API endpoint URL.
- `parameters` : API request parameters. Refer to [#接口说明(Interface Documentation)](https://developer.hitokoto.cn/sentence/#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E) .
- `from_where` : Whether to display the source of the sentence.

Example Configuration File:

```json
{
    "interval": "1m",
    "parameters": {
        "c": ["a", "c"],
        "max_length": 10
    },
    "base_url": "https://v1.hitokoto.cn/",
    "from_where": true
}
```



### API 调用

The plugin provides a `get_hitokoto()` function to call the API.

Usage Example:

```python
import hitokoto

message = hitokoto.get_hitokoto()
print(message)
```


### Download

> [!IMPORTANT]
> Read the README file in plugin repository before using it.

*Data fetching failed*

