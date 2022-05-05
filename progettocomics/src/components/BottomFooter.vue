<template>
<div class="footer-bottom">
    <div class="Container-social">
        <div class="button">
            <button>SING-UP NOW!</button>
        </div>
        <div class="social">
            <p>FOLLOW US</p>
            <img v-for="(IconS, index) in IconSocial" :key="index" :src="IconS.img" alt="" srcset="">
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'BottomFooter',
    data() {
        return{
            IconSocial:[
                {
                    img: require('../assets/footer-facebook.png')
                },
                {
                    img: require('../assets/footer-periscope.png')
                },
                {
                    img: require('../assets/footer-pinterest.png')
                },
                {
                    img: require('../assets/footer-twitter.png')
                },
                {
                    img: require('../assets/footer-youtube.png')
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/StyleAbsolute';

.footer-bottom{
    background-color: rgb(45, 45, 45);
    height: 10vh;
}

.Container-social{
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

button{
    border-color:$BackgroundIcons;
    padding: 10px 14px;
    background-color: transparent;
    color: white;
}

.social{
    display: flex;
}

img{
    padding:0 5px;
}

p{
    color:$BackgroundIcons;
    font-weight: bold;
    line-height: 2;
    padding:0 5px;
}
</style>