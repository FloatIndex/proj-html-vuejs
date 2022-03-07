<template>
  <header class="container">
      <nav>
            <a href="#"><img class="logo" src="../assets/images/logotype.png"></a>
            <MyMenu />
      </nav>
  </header>
</template>

<script>
import MyMenu from './partials/MyMenu.vue';

export default {
    name: 'MyHeader',
    components: {
        MyMenu
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

header {
    height: 80px;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    z-index: 999;
    color: $lightGrey;

    nav {
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
            height: 12px;
        }
    }
}
</style>