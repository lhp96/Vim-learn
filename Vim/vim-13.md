# Day13

## 目标：替换字符串
- 替换命令:   `:[range]s[ubstitue]/{pattern}/{string}/[flags] `
- 全局替换  `:%s/vnode/haha<Enter>`  只会替换每行第一个
- 真全局替换 `:%s/vnode/haha/g<Enter>`  
- 多选操作： `gb`  按gb几次就选中多少个，区别大小写