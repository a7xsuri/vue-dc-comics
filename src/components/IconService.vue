<template>
    <div class="Container-icons">
        <div class="container">
            <div class="icon" v-for="(Icon, index) in Service" :key="index">
                <img :src="Icon.img" alt="{Icon.img}">
                <p>{{Icon.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>

export default{
    name: 'IconService',
    data() {
        return{
            Service:[
                {
                    img: require('../assets/buy-comics-digital-comics.png'),
                    text: 'DIGITAL COMICS',
                },
                {
                    img: require('../assets/buy-comics-merchandise.png'),
                    text: 'DC MERCHANDISE',
                },
                {
                    img: require('../assets/buy-comics-digital-comics.png'),
                    text: 'SUBSCRIPTION',
                },
                {
                    img: require('../assets/buy-comics-shop-locator.png'),
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    img: require('../assets/buy-dc-power-visa.svg'),
                    text: 'DC POWER VISA',
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/StyleAbsolute';

.Container-icons{
    background-color: $BackgroundIcons;
    height: 25vh;
    
    .container{
        display: flex;
        justify-content: space-around;
        align-items: center;
        width:80%;
        margin: 0 auto;
        height:100%;
    }

    .icon{
        display: flex;

        img{
            height: 60px;
        }
        p{
            color:white;
            line-height:3.5;
            padding-left: 10px;
        }
    }
}
</style>
