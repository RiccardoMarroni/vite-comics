<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
        <!-- <CardComponent :tumb="item.src" :price="item.price" :seriece="item.seriece" type="item.type" /> -->
        parixiale
        </div>
    </main>
</template>

<script>
import {comics} from '../data/store.js'; //import dei dati
import CardComponent from '../components/CardComponent.vue';
    export default {
        name: 'MainComponent',
        components:{
            CardComponent
        },
        data() {
            return{
                products: comics
            }
        },
        mounted(){
            console.log(this.products);
        }
    }
    
     
</script>



<style lang="scss" scoped >
main{
    background-color: black;
    height: auto;
    color:white;
    margin-top: 50px;
}

.jumbotron{
    background-image: url('/img/jumbotron.jpg'), url('/img/jumbotron.jpg');
    background-size: cover;
    padding: 200px;
        
        
}
</style>