# 键盘侠养成记

- 学完 Vim，可以带你装 B 带你飞，实现真正的键盘侠
- 推荐使用 mac 配套使用体验更佳，没有就快买！！！

## 目录

- Vim 基本操作
- VSCode 使用快捷键
- Chrome 使用快捷键

## vscode + vim 常用

### 单词

- `diw`  删除这个单词
- `ciw`  删除这个单词并进入 ins
- `yiw`  复制这个单词
- `daa`  删除函数一个参数
- 组合：
  - 删除当前单词：cw
  - 在当前单词结尾处添加：ea

### 搜索一个字符串

- `*` or  `#`  将光标放在单词上，就能开始搜索,按一次之后：n 向下找, N 向上找
- `/test<Enter>`   n:下一个 N:上一个
- `fxx`  根据前 2 个字母查找 `;`下一个 `,`上一个

### 函数

- `gd`   查看函数的创建和使用的地方，配合 `Ctrl o` 再返回原来的位置
- `gh`   查看函数的签名
- `fn`   生成纯 function
  - `function name(params) {}`
- `anfn` 生成箭头函数（tab 可以跳到下个位置）
  - `(params) => {}`
- `ef` 导出函数
  - `export function member (arguments) {}`
- `nfn` 有 const 的箭头函数
  - `const add = (params) => {}`

### 快速移动

- 向下： Ctrl + f  /  `J`   /  `<space><space>j`  /  `<space><space>w`
- 向上： Ctrl + b  /  K  /  `<space><space>k`

### 文件

- 复制当前文件路径  `cmd + k + p`
