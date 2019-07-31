# vue-calendar-mobile
仿安网易云音乐地区选择，二级联动选择插件  
基于 CLI3 开发

### 开发目的

>复刻网易云安卓客户端用

### 用法

```html
<template>
  <div>
    <areaWin :provCode.sync="provCode" :cityCode.sync="cityCode" :provName.sync="provName" :cityName.sync="cityName" :areaShow.sync="areaShow"></areaWin>
  </div>
</template>

<script>
  import areaWin from './area-select.vue'
  export default {
    data() {
      return {
        areaShow: false,
        provCode: 510000,
        provName: '广东省',
        cityCode: 510100,
        cityName: '广州市'
      }
    },
    components: { areaWin }
  }
</script>

```

### 说明
>所有参数都是同步的修改的