<template>
  <MainHeader></MainHeader>
  <NoticeBtn></NoticeBtn>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import MainHeader from './components/main-header.vue'
import NoticeBtn from './components/notice-btn.vue';



@Options({
  components: {
    MainHeader,
    NoticeBtn,
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  
}
</style>
