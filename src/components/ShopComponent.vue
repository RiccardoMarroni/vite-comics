<template>
    <div class="back-shop">
        <div class="container">
            <ul class="d-flex">
                <li v-for="(item, index) in ShopLink" :key="index">
                <a :href="item.url">{{ item.label }}</a>
            </li>
            </ul>
        </div>
    </div>
</template>

<script>
   export default {
        name: 'ShopComponent',
        data() {
            return{
                ShopLink : [
                    {
                        
                        label:"DIGITAL COMICS",
                        url:"#",
                    },
                    {
                        label:"DC MERCHANDASING",
                        url:"#",
                    },
                    {
                        label:"SUBSCRIPTION",
                        url:"#",
                    },
                    {
                        label:"COMIC SHOP LOCATOR",
                        url:"#",
                    },
                    {
                        label:"DC POWER VISA",
                        url:"#",
                    },
                ]
            }
        }
    }
    
</script>

<style lang="scss" scoped>
ul{
    justify-content: center;
    

    li{
        
        a{
            color: white;
            padding-top: 35px;
        }
    }
}
</style>