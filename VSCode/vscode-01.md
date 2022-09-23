# Day15

## 目标：掌握窗口的管理

- `Command + ;` 新建一个右窗口 原：Command + \
- `Command + Ctrl + ;` 新建一个下窗口 (少用)
- `Command + w` 关闭一个窗口
- `Shift + 方向键` 窗口切换

- 配置文件如下

```json
{
    "key": "ctrl+cmd+;",
    "command": "workbench.action.splitEditorUp"
},
{
    "key": "shift+left",
    "command": "vim.remap",
    "when": "vim.mode == 'Normal'",
    "args":{
        "after": ["<c-w>", "h"]
    }
},
{
    "key": "shift+right",
    "command": "vim.remap",
    "when": "vim.mode == 'Normal'",
    "args":{
        "after": ["<c-w>", "l"]
    }
},
{
    "key": "shift+up",
    "command": "vim.remap",
    "when": "vim.mode == 'Normal'",
    "args":{
        "after": ["<c-w>", "k"]
    }
},
{
    "key": "shift+down",
    "command": "vim.remap",
    "when": "vim.mode == 'Normal'",
    "args":{
        "after": ["<c-w>", "j"]
    }
}

```
