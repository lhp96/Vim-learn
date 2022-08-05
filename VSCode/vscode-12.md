# Day 29

## 目标：终端

- 打开终端
  - ctrl + `
  - 改为：`ctrl + ,`
  - workbench.action.terminal.toggleTerminal
- 清空终端
  - `cmd + k`
- 分屏
  - `cmd + ;` 向右新建
  - `cmd + [ ` or `cmd + ]`分屏切换
  - workbench.action.terminal.focusNextPane
  - workbench.action.terminal.focusPreviousPane
- 关闭当前终端窗口
  - `ctrl + w`
  - workbench.action.terminal.kill
- 新建终端
  - `ctrl + n`
  - workbench.action.terminal.new
- 窗口切换
- `shift + cmd + [` or `shift + cmd + ]`

## 拓展：直接打开终端 app

- `shift + cmd + c`
  配置文件修改
  settings.json

```json
  "terminal.external.osxExec": "iTerm.app",
```
