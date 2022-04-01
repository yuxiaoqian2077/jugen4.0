<template>
  <div class="hello">
    
    
    
    <el-button type="primary" @click="open1">
    <el-icon style="vertical-align: middle;">
      <Message />
    </el-icon>
    <span style="vertical-align: middle;"> notice </span>
  </el-button>
    
    
    
  </div>
</template>

<script lang="ts" setup>

import {ElNotification} from 'element-plus'
import {ElIcon} from 'element-plus'
import { h } from 'vue';
import {Message} from '@element-plus/icons-vue'
const open1 = () => {
  ElNotification.success({
    title: 'notice',
    message: h('i', { style: 'color: green' }, 'notice'),
    duration: 2000,
  })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
