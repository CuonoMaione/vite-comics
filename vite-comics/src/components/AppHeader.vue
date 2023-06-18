<script>
export default{
    name: "AppHeader",
    components: {
        NavLink
    },
    data() {
        return {
           headList: [
                {
                    link: "#",
                    text: "Characters",
                },
                {
                    link: "#",
                    text: "Comics",
                },
                {
                    link: "#",
                    text: "Movies",
                },
                {
                    link: "#",
                    text: "Tv",
                },
                {
                    link: "#",
                    text: "Games",
                },
                {
                    link: "#",
                    text: "Collectibles",
                },
                {
                    link: "#",
                    text: "Videos",
                },
                {
                    link: "#",
                    text: "Fans",
                },
                {
                    link: "#",
                    text: "News",
                },
                {
                    link: "#",
                    text: "Shop",
                },
            ]
        };
    },
    components: { NavLink }
}

import NavLink from './NavLink.vue';



</script>

<template>
    <header>

        <img src="../assets/img/dc-logo.png" alt="">

     
            <NavLink v-for="element in headList" :linkText="element.text" :linkWeb="element.link"/>
            
    </header>

</template>

<style lang="scss" scoped>
header{
    width: 70%;
    margin: 0 auto;

    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 1rem;
}

img{
    height: 80px;
}




</style>