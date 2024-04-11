<!-- MOLISANA -->


<template>
    <main>
        <div class="container">
            <h2 >lista prodotti</h2> 
            <div class="row">
                <div class="col-12" v-for="(item, index) in products" :key="index" >
                    <CardTest />
                </div>
            </div>
            
        </div>
    </main>
</template>

<script>
import {prodotti} from '../data/store.js'; //import dei dati
import CardTest from '../component/CardTest.vue';
    export default {
        name: 'MainComponent',
        data() {
            return{
                products: prodotti
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
    height: 200px;
    color:white;
    margin-top: 50px;
}
</style>