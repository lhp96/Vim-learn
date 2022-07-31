# Day 24

## 目标：搞定 git

- 显示 source control 面板
  - `<leader> g g`
- Stage change `git add 当前文件`
  - `<leader> g s`
- commit
  - `<leader> g c`
- diff
  - `<leader> g d f`
- Unstage change
  - `<leader> g u`
- Discard change `在git add 之前使用`
  - `<leader> g c l`
- vscode 插件
  - edamagit 插件，简化 git 操作，减少使用终端

## git 拓展

- lazygit 是终端中的 git 图形化界面
  - `brew install lazygit`
  - or `brew install jesseduffield/lazygit/lazygi`
- `echo "alias lg='lazygit'" >> ~/.zshrc`
- 记录一些基础操作
- 块间移动
  - `h`, `l`
  - `数字键 1 2 3 4 5`
  - 鼠标点击
- 块内移动 `j`, `k`
- stage changed 在`Files`中`space`
- 在 files 下 `c` 可以`commit`操作 录入后回车
- reset 在`Commits`中`space`
- 进入`已暂存更改`, `enter`
- 通过`tab`切换区域，按空格来选择 stage change 和 unstage change，分开提交

- 重要，查看帮助 `?`
