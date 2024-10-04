---
excalidraw-plugin: parsed
excalidraw-linkbutton-opacity:
---
greet:: Hello World!

- [ ] `= this.greet`

```dataviewjs
const page = dv.current()
const inlineGreet = page["greet"]

console.log(inlineGreet)
dv.header(2, inlineGreet)
dv.list([inlineGreet])
dv.el("span", `- [ ] ${inlineGreet}`)
dv.taskList(page.file.tasks)
dv.table(["问候"], [[inlineGreet]])
```




---
---
description: 测试描述
tags:
  - 标签1
  - 标签2
---

inlineProp1:: 测试
inline_test:: 下划线命名测试
InlineTest2:: 大写字母开头命名测试
Test Long Split Words:: 不规则变量名测试
**Bold Text**:: 加粗文本测试
这是内联字段 [inlineProp2:: 在文本内部]
我的名称不可见 (inlineProp3:: 我的变量名不可见)
- 在列表中定义标签 #标签3 和内联变量 [inlineProp4:: 在列表内]
- [ ] 在任务中定义标签 #标签4 和内联变量 [inlineProp5:: 在任务内]
外链：[[2022-01-06]]



参考：
[Obsidian 达人成长之路 #2：使用终极工具 Dataview 释放笔记库的潜力 · JavaScript API - wujie520303 - SegmentFault 思否](https://segmentfault.com/a/1190000044914813)

```dataviewjs
Object.keys(dv.current()).forEach(key => {
    console.log(key);
})
```
```dataviewjs
Object.keys(dv.current()).forEach(key => {
    console.log(key);
})
```