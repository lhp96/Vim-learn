### Day18

## 目标：调用 vscode 的命令

1. commands 字段

- `"command":[{}, { "command": "字符串", xxxx: XXX }]` 对象数组
- `"command": "command ID"`

2. 格式化文档

- 原：`shift + alt + f`
- 后：`<leader> + f + d`

3. 重命名

- 原：`F2`
- 后：`<leader> + f + n`

4. 折叠代码

- 原：`alt + cmd + [`
- 后：`<leader> + [`

5. 思想

- 打开键盘快捷方式 -> 搜索你想替换的东西 -> 右键 Copy Çommand ID
- 再修改 settings.json 文件 就行了

配置文件修改

```json
  "vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": ["<leader>", "f", "d"],
      "commands": ["editor.action.formatDocument"]
    },
    {
      "before": ["<leader>", "r", "n"],
      "commands": ["editor.action.rename"]
    },
    {
      "before": ["<leader>", "["],
      "commands": [
        {
          "command": "editor.fold"
        },
        {
          "command": "vim.remap",
          "args": {
            "after": ["$", "%"]
          }
        }
      ]
    }
  ],
```
