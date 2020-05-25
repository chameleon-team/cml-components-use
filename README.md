title:如何引用原生组件
---
### 在多态组件中引入原生组件
```json
{
  "base": {
    "usingComponents": {
      "ori-comp":"../ori-comp/ori-comp",
      "vant-button":"vant-weapp/dist/button/index"
    }
  }
}
```

### 在多态组件中使用

```html
<template>
  <view>
    <text>wx端自定义组件</text>
    <ori-comp></ori-comp>
  
  </view>
</template>
```

引用对应端的原生组件的时候，一定要在对应端的多态组件中使用，不要在 xxx.cml 文件中直接使用