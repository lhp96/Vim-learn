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
- 块间移动
  - `h`, `l`
  - `数字键 1 2 3 4 5`
  - 鼠标点击
- 块内移动
  - `j`, `k`
- stage changed `add`
  - 在`Files`中`空格`
  - `a` 全部 add
- commit
  - 在`Files`下 `c` 录入后回车
- reset
  - 在`Commits`中`空格`
- 取消
  - `d` or `D`
- pull `p` &nbsp; push `P`

- 通过`tab`切换区域，按空格来选择 stage change 和 unstage change，分开提交

- 重要，查看帮助 `?`

- 工作
  - `p a c "xxx" 回车 P`