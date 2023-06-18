<script>

export default{
    name: 'NavLink',
    props: {
        linkText : String ,
        linkWeb : String ,
    },
    
}
</script>

<template>
    
    <ul>
         <li> 
            <a :href=" linkWeb "> {{ linkText }} </a> 
        </li> 
    </ul> 
    
</template>

<style scoped lang="scss">
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