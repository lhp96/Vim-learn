# Day 27

## 目标：掌握重构

## `cmd + .` 呼出重构菜单

1. 配合插件丰富重构功能

- abracadabra
- hocus pocus
- javascript booster

2. 使用场景

- 选择代码块重构成函数
  - 选中之后，`cmd + .`
- 将字符串提炼成**变量**
  - console.log("ccc") =>
  - `const ccc = "ccc"; console.log(ccc);`
- 内联->跟提炼变量相反
- 创建函数
  - `空格 ff`
- 创建变量
  - `空格 vv`
- 将 function 转化为 箭头函数（互换）
- 将 if/else 转化为 三目运算符 （互换）

## tips

- 创建函数和创建变量，是先定义好你要用的东西，再使用命令创建好，先声明后使用(先用后付)

配置文件修改
settings.json

```json
    {
      "before": ["<Leader>", "f", "f"],
      "commands": ["hocusPocus.createFunction"]
    },
    {
      "before": ["<Leader>", "v", "v"],
      "commands": ["hocusPocus.createVariable"]
    }
```
