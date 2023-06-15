<script>
export default{
    name: 'AppHeader',
    data(){
        return{
            headList : [
                {
                    link: '#',
                    text: 'Characters',
                },
                {
                    link: '#',
                    text: 'Comics',
                },
                {
                    link: '#',
                    text: 'Movies',
                },
                {
                    link: '#',
                    text: 'Tv',
                },
                {
                    link: '#',
                    text: 'Games',
                },
                {
                    link: '#',
                    text: 'Collectibles',
                },
                {
                    link: '#',
                    text: 'Videos',
                },
                {
                    link: '#',
                    text: 'Fans',
                },
                {
                    link: '#',
                    text: 'News',
                },
                {
                    link: '#',
                    text: 'Shop',
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <ul>
            <li v-for="element in headList">
                <a :href=" element.link ">{{ element.text }}</a>
            </li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
ul{
    display: flex;
    list-style: none;
    
    li{
        margin-right: 0.5rem; 
        a{
            text-decoration: none;
            color: black;
        }
    }
    
}
</style>