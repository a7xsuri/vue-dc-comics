<template>
    <div class="ThumbCard">
        <img :src="immagine" :alt="titolo">
        <h3>{{titolo}}</h3>
    </div>
</template>

<script>
export default{
    name: 'SeriesCard',
    data() {
        return{

        }
    },
    props: ['immagine', 'titolo']
}
</script>

<style lang="scss" scoped>
@import '../style/StyleAbsolute';

.ThumbCard{
    width:15%;
}

h3{
    color:white;
}

img{
    width: 150px;
    height: 150px;
    object-fit: cover;
}

</style>
