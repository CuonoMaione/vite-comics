<template lang="">
    <div class="cards">
                
                <img :src="cardImage" alt="">
                <h2>{{ cardTitle }}</h2>

    </div>
</template>
<script>
export default {
    name: 'CardComics',
    props:{
        cardImage : String ,
        cardTitle : String ,
    }
}
</script>
<style lang="scss" scoped>
    div.cards{
        width: calc((100%/6) - 1rem);
        margin-left: 1rem;
        margin-bottom:2rem;
        
        
    }

    img{
        width: 100%;
        height: 160px;
        object-fit:cover;
        object-position: top;
    }

    h2{
        font-size: 0.8rem;
        padding-top:0.5rem;
        text-transform: uppercase;
    }
</style>