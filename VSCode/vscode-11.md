# Day 28

## 目标：VSpaceCodei 插件

1. 初始化

- settings
  - [settings.json](https://github.com/VSpaceCode/VSpaceCode/blob/master/src/configuration/settings.jsonc)
- keybandings
  - [keybandings.json](https://github.com/VSpaceCode/VSpaceCode/blob/master/src/configuration/keybindings.jsonc)

2. 在这基础上修改 快捷键
3. 自定义

   - 快捷键
   - 呼出内容 `空格 + ;`

4. 配置文件修改

```json
    {
        "key": "space",
        "command": "vspacecode.space",
        "when": "activeEditorGroupEmpty && focusedView == '' && !whichkeyActive && !inputFocus"
    },
    // Trigger vspacecode when sidebar is in focus
    {
        "key": "space",
        "command": "vspacecode.space",
        "when": "sideBarFocus && !inputFocus && !whichkeyActive"
    },
```
