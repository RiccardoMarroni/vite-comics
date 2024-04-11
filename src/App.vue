<template>
  <HeaderComponent />
  <MainComponent />
  <ShopComponent />
  <JumboFooter />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import ShopComponent from './components/ShopComponent.vue';
import JumboFooter from './components/JumboFooter.vue';
import FooterComponent from './components/FooterComponent.vue';


  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
      ShopComponent,
      JumboFooter,
      FooterComponent
    },
    data(){
      return{

      }
    }
  }
</script>

<style lang="scss" scoped>

</style>