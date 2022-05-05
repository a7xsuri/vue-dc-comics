<template>
  <div id="app">
    <HeaderMenu/>
    <JumboImage/>
    <IconService/>
    <TopFooter/>
    <BottomFooter/>
  </div>
</template>

<script>
import HeaderMenu from './components/HeaderMenu.vue'
import JumboImage from './components/JumboImage.vue'
import IconService from './components/IconService.vue'
import TopFooter from './components/TopFooter.vue'
import BottomFooter from './components/BottomFooter.vue'

export default {
  name: 'App',
  components: {
    HeaderMenu,
    JumboImage,
    IconService,
    TopFooter,
    BottomFooter,
  }
}
</script>

<style lang="scss" scoped>
@import './style/StyleAbsolute';
body{
    margin: 0;
}
</style>
