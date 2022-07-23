### Day19

## 目标：操作文件

#### 窗口焦点切换

1. 切到 files explorer `Ctrl + ;`
2. 切到 editor `Ctrl + '`
3. 移动光标 `j k`
4. 折叠/展开 `h / l`
5. 创建文件/文件夹 `a / A`
6. 重命名 / 删除 `r / n`

在之前的课程中，我们学习了 vim 的窗口管理的一些命令，当光标在编辑窗口时，我们通过 shift + ctrl + h / l 来使光标在左右窗口移动焦点，不过在使用的过程中这个快捷键还是比较不顺手，毕竟要按三个键，而且 vim 的命令只能在编辑窗使用，如果我们当前焦点在终端的时候，就无法使用 vim 的命令切换焦点了；而对于我们日常来说，需要聚焦到侧边的资源管理器的情况是很常有的，因此我们需一个更方便更通用的组合键达到这个目的；而 vscode 中，其实是有这个快捷键的，就是 shift + command + e，既然如此就可以通过 command + shift + p 并且搜索 “Open keyboard shortcuts” 找到 keybindings.json 文件添加映射：

配置文件修改

```json

  {
    "key": "ctrl+;",
    "command": "workbench.view.explorer"
  },
  {
    "key": "ctrl+'",
    "command": "workbench.action.focusFirstEditorGroup"
  },
  {
    "key": "a", // 新建文件
    "command": "explorer.newFile",
    "when": "filesExplorerFocus && !inputFocus"
  },
  {
    "key": "shift+a", // 新建文件夹
    "command": "explorer.newFolder",
    "when": "filesExplorerFocus && !inputFocus"
  },
  {
    "key": "d",
    "command": "deleteFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "r",
    "command": "renameFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  }

```

```json
"vim.normalModeKeyBindingsNonRecursive": [
  {
    "before": ["<Leader>", "n", "d"],
    "commands": ["explorer.newFolder"]
  },
  {
    "before": ["<Leader>", "n", "f"],
    "commands": ["explorer.newFile"]
  },
]
```
