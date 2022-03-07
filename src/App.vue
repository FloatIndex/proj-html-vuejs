<template>
  <div id="app">
    <MyHeader :menu="menuList"/>
    <MyMain/>
    <MyFooter :menu="menuList"/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  data() {
    return {
      menuList: [
        'home',
        'about',
        'projects',
        'services',
        'blog',
        'contact'
      ]
    }
  },
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  }
}
</script>

<style lang="scss">
@import './assets/style/general.scss';

#app {
  position: relative;
}
</style>
