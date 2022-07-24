# Day12

## 目标：处理包裹字符的符号

- vim-surround
- cs `<existing><desired>`
- ys `<motion><desired>`
- ds `<existing>` ：
- 可视化模式下 `S`+ 符号 给字符串加上符号

## 练习

```
import add from "./add"
ysiw{    修改后：{ add }

const a = "b${name}"
cs + "(  修改后：( b${name} )

x = (a + b) * c;
ds + (   修改后：a + b * c
```
