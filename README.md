# 简介

基于Vue 2.x 开发的Avatar 裁切上传插件

## 使用方法

main.js

```js
import Vue from 'vue'
import AvatarCrop from 'vue-avatar-crop'

Vue.use(AvatarCrop)
```

app.vue

```js
<template>
  <div>
    <a @click="show = true"></a>
    <AvatarCrop field="img" v-model="show" :width="256" :height="256" url="/upload" img-format="png"></AvatarCrop>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        show: false
      }
    }
  }
</script>
```

