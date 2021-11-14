---
import: 
  import { Select, SelectOptions } from 'otaku-ui'
---

[[toc]]

## Select 下拉框

::: demo

简单的评分

```tsx
<Select>
{
  new Array(20).fill().map((_, index) => {
    return <SelectOptions key={index}>第{index + 1}个选项</SelectOptions>
  })
}
</Select>
```
:::