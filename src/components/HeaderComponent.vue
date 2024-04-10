<template>
    <header class="container justify-content-between d-flex" >
       <a> <img src="..\assets\img\dc-logo.png" alt="logo"> </a>
       <ul>
        <li v-for="(item, index) in headerLink" :key="index">
                <a :href="item.url">{{ item.label }}</a>
            </li>
    </ul>
    </header>
</template>

<script>
    export default {
        name:'HeaderComponent',
        data(){
            return{
                headerLink: [
    {
        label:"characters",
        url:"#",
        
    },
    {
        label:"comics",
        url:"#",
        
    },
    {
        label:"movies",
        url:"#",
        
    },
    {
        label:"tv",
        url:"#",
        
    },
    {
        label:"games",
        url:"#",
       
    },
    {
        label:"collectibles",
        url:"#",
        
    },
    {
        label:"videos",
        url:"#",
        
    },
    {
        label:"fans",
        url:"#",
        
    },
    {
        label:"news",
        url:"#",
        
    },
    {
        label:"shop",
        url:"#",
        
    }
]
            }
        }
    }
</script>

<style >
ul{
    display: flex;
    list-style: none;
    height: 100%;
    color: black;
    
    li{
        display: flex;
        align-items: center;
        height: 100%;
        margin: 0 10px;
        &:hover, &.active{
            border-bottom: 5px solid blue;
            cursor: pointer;
        }
        
        &:hover a {
            color: black;
        }
        a{
            text-decoration: none;
            text-transform: uppercase;
            font-weight: 600;
            font-size: .9rem;
            color: $main-grey;
        }
    }
}

</style>