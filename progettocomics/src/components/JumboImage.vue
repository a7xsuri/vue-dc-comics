<template>
    <div id="jumbo">
        <div class="text">
            <p> -- CONTENT GOES HERE -- </p>
        </div>
    </div>
</template>

<script>
export default{
    name: 'JumboTron',
    data() {
        
    },
}
</script>

<style lang="scss" scoped>
@import '../style/StyleAbsolute';
#jumbo{
    background-color: $BackgroundJumbo;
    height: 90px;
}

.text{
    width: 80%;
    margin:0 auto;
}

    p{
        color: white;
        line-height: 5;
    }
</style>