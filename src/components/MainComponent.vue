<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
            <h2 >lorem500</h2> 

        </div>
    </main>
</template>

<script>
import {comics} from '../data/store.js'; //import dei dati

    export default {
        name: 'MainComponent',
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