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
    
    li{
         
        a{
            text-decoration: none;
            color: #47474f;
            text-transform: uppercase;
        }
    }
    
</style>