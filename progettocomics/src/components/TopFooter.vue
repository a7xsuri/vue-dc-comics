<template>
    <div class="top-footer">
      <div class="menu-footer">
        <div class="menu">
      <ul>
        <li class="macro">DC COMICS</li>
        <li v-for="(VoiceMenu, index) in MenuComics" :key="index">{{VoiceMenu.text}}</li>
      </ul>
      <ul>
        <li class="macro">SHOP</li>
        <li v-for="(VoiceMenu, index) in MenuShop" :key="index">{{VoiceMenu.text}}</li>
      </ul>
      </div>
      <ul>
        <li class="macro">DC</li>
        <li v-for="(VoiceMenu, index) in MenuDC" :key="index">{{VoiceMenu.text}}</li>
      </ul>
      <ul>
        <li class="macro">SITES</li>
        <li v-for="(VoiceMenu, index) in MenuSites" :key="index">{{VoiceMenu.text}}</li>
      </ul>
      </div>
    </div>
</template>

<script>

export default {
  name: 'TopFooter',
  data(){
    return{
      MenuComics:[
      {
      text: "Characters",
      active: false,
    },
    {
      text: "Comics",
      active: true,
    },
    {
      text: "Movies",
      active: false,
    },
    {
      text: "Tv",
      active: false,
    },
    {
      text: "Games",
      active: false,
    },
    {
      text: "Collectibles",
      active: false,
    },
    {
      text: "Video",
      active: false,
    },
    {
      text: "Fans",
      active: false,
    },
    {
      text: "News",
      active: false,
    },
    {
      text: "Shop",
      active: false,
    }
      ],
      MenuShop:[
      {
      text: "Shop DC",
      active: false,
    },
    {
      text: "Shop DC Collectibles",
      active: true,
    },
      ],
      MenuDC:[
      {
      text: "Terms Of Use",
      active: false,
    },
    {
      text: "Privacy policy (New)",
      active: true,
    },
    {
      text: "Ad Choices",
      active: false,
    },
    {
      text: "Adverising",
      active: false,
    },
    {
      text: "Jobs",
      active: false,
    },
    {
      text: "Subscriptions",
      active: false,
    },
    {
      text: "Talent Workshops",
      active: false,
    },
    {
      text: "CPSC Certificates",
      active: false,
    },
    {
      text: "Ratings",
      active: false,
    },
    {
      text: "Shop Help",
      active: false,
    },
    {
      text: "Contact Us",
      active: false,
    }
      ],
      MenuSites:[
      {
      text: "DC",
      active: false,
    },
    {
      text: "MAD Magazine",
      active: true,
    },
    {
      text: "DC Kids",
      active: false,
    },
    {
      text: "DC Universe",
      active: false,
    },
    {
      text: "DC Power Visa",
      active: false,
    },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../style/StyleAbsolute.scss';

.top-footer{
  height: 50vh;
  background-image: $BackgroundFooterTop;

  .menu-footer{
  width: 80%;
  display: flex;
  margin: 0 auto;
  }

  ul{
    list-style: none;
    color:rgb(174, 174, 174);
    padding:20px 10px;

    .macro{
      font-weight: bold;
      padding-bottom: 10px;
      color:white
    }
  }
}
</style>