<script>
export default{
    name: 'AppFooter',
    data(){
        return{
            headList : [
                {
                    link: '#',
                    text: 'DC COMICS',
                },
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
            ],
            shopList : [
                {
                    link:'#',
                    text:'Shop DC'
                },
                {
                    link:'#',
                    text:''
                }
            ]

        }
    }
}
</script>

<template>
    <footer>
        <section class="upper-footer"> 
            <div class="container-footer">
                <ul>
                    <li v-for="element in headList">
                        <a :href=" element.link ">{{ element.text }}</a>
                    </li>
                </ul>
            </div> 
        </section>      
    </footer>
</template>

<style lang="scss" scoped>
    .upper-footer{
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
    }

    .container-footer{
        width: 70%;
        margin: 0 auto;
    }

    ul{
    display: flex;
    flex-direction: column;
    list-style: none;
        li{
            margin-right: 0.5rem; 
            font-size: 0.7rem;
            a{
                text-decoration: none;
                color:gray;
                
        } 
        }
    }
    li{
        margin-right: 0.5rem; 
        a{
            text-decoration: none;
            color: black;
            
            
    } 
    }
    li:first-child{
        font-size: 2rem;
        text-transform: uppercase;
        a{
            color: white;
        }

    }

</style>