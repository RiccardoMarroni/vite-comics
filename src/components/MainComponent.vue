<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
            <h3 class="title text-center">Current Series</h3>
         <CardComponent :item="comics"/> 
        
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
                 comics
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

h3{
    color:white;
    background-color: blue;
    margin: 0, 60px;
}
</style>