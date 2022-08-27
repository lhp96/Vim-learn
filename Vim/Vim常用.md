## 单词

- `diw` 删除这个单词
- `ciw` 删除这个单词并进入 ins
- `yiw` 复制这个单词
- `daa` 删除函数一个参数

## 括号

- `dib` 删除括号中的内容
- `dab` 删除括号及其内容
- `diB` 删除{}中的内容
- `dsb` 删除括号 `ds{` &nbsp;`ds[`
- `ysiw(` 添加括号 &nbsp;`cs{(` 修改括号
- `v2aB` 选择`{{}}`的内容 {{sfad.count}}

## 搜索一个字符串

- `*`&nbsp;/&nbsp;`#` 将光标放在单词上，就能开始搜索,按一次之后：n 向下找, N 向上找
- `/test<Enter>` n:下一个 N:上一个
- `fxx` 根据前 2 个字母查找 `;`下一个 `,`上一个

## 函数 (依赖 vscode 插件)

- `fn` 生成纯 function
  - `function name(params) {}`
- `anfn` 生成箭头函数（tab 可以跳到下个位置）
  - `(params) => {}`
- `ef` 导出函数
  - `export function member (arguments) {}`
- `nfn` 有 const 的箭头函数
  - `const add = (params) => {}`

## 查看函数的定义

- `gd` &nbsp; 配合 `Ctrl o` 再返回原来的位置

## vscode 插件

- Vue VSCode Snippets
- Vue 3 Snippets
- JavaScript (ES6) code snippets
- JavaScript standardjs styled snippets
