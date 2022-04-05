<template>
  <div class="hello">
    
    
    
    <el-button type="primary" @click="open1">
    <el-icon style="vertical-align: middle;">
      <shopping-cart />
    </el-icon>
    <span style="vertical-align: middle;"> 购买 </span>
  </el-button>
    
    
    
  </div>
</template>

<script lang="ts" setup>

import {ElNotification} from 'element-plus'
import {ElIcon} from 'element-plus'
import { h } from 'vue';
import {ShoppingCart} from '@element-plus/icons-vue'
const open1 = () => {
  ElNotification.success({
    title: '成功',
    message: h('p', { style: 'color: green' }, '购买成功！'),
    duration: 2000,
  })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
