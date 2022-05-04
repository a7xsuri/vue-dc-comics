<template>
  <div class="header-menu">
    <img src="../assets/dc-logo.png" alt="logo dc">
    <nav>
      <ul>
        <li v-for="(PageMenu, index) in NavItems" :key="index" :class="{'active': PageMenu.active}">{{PageMenu.text}}</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HeaderMenu',
  data(){
    return {
      NavItems:[
    {
      text: "CHARACTERS",
      active: false,
    },
    {
      text: "COMICS",
      active: true,
    },
    {
      text: "MOVIES",
      active: false,
    },
    {
      text: "TV",
      active: false,
    },
    {
      text: "GAMES",
      active: false,
    },
    {
      text: "COLLECTIBLES",
      active: false,
    },
    {
      text: "VIDEO",
      active: false,
    },
    {
      text: "FANS",
      active: false,
    },
    {
      text: "NEWS",
      active: false,
    },
    {
      text: "SHOP",
      active: false,
    }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/StyleAbsolute';

.header-menu{
  width: 80%;
  margin: 0 auto;
  display:flex;
  justify-content: space-between;
  margin-bottom: 10px;


  ul{
  list-style: none;
  height: 100%;
  display: flex;
  align-items: center;

    li{
      margin:0px 10px;
    }
  }

}

.active{
  border-bottom: 1px solid blue;
}
</style>
