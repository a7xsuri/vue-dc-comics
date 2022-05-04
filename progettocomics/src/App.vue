<template>
  <div id="app">
    <HeaderMenu/>
    <JumboImage/>
    <IconService/>
  </div>
</template>

<script>
import HeaderMenu from './components/HeaderMenu.vue'
import JumboImage from './components/JumboImage.vue'
import IconService from './components/IconService.vue'

export default {
  name: 'App',
  components: {
    HeaderMenu,
    JumboImage,
    IconService
  }
}
</script>

<style lang="scss" scoped>
@import './style/StyleAbsolute';

</style>
