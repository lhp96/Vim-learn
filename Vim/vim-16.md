### day16

## 目标：如何删除一个函数

- `%` 匹配括号
- vim-indent-object 删除一个函数 =>前提：代码格式化
  - `vai` 在函数内使用
  - `dai` &nbsp;/ &nbsp;`dai`
  - `v$%d` 在函数头使用

```js
function aaa(x, y, s) {
  const res = { x, y, s };
}

const test = (a = 1) => {
  console.log(a);
  a = 2;

  settimeout(() => {
    console.log(a);
  }, 500);
};
```
