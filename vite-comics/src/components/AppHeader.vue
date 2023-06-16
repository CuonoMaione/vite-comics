<script>
export default{
    name: "AppHeader",
    components: 'NavLink',
    data() {
        return {
           props: {
            
           }
        };
    },
    components: { NavLink }
}

import NavLink from './NavLink.vue';



</script>

<template>
    <header>

        <img src="../assets/img/dc-logo.png" alt="">

        <ul>
            <li v-for="element in headList">
                <a :href=" element.link ">{{ element.text }}</a>
            </li>
        </ul>
    </header>

    <NavLink>
    </NavLink>
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

ul{
    display: flex;
    
    list-style: none;
    
    li{
        margin-right: 0.5rem; 
        a{
            text-decoration: none;
            color: black;
            text-transform: uppercase;
        }
    }
    
}


</style>