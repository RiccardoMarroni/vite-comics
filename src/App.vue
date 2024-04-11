<template>
  <HeaderComponent />
  <MainComponent />
  <ShopComponent />
  <JumboFooter />
  <BottomFooter />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import ShopComponent from './components/ShopComponent.vue';
import JumboFooter from './components/JumboFooter.vue';
import BottomFooter from './components/BottomFooter.vue';
import FooterComponent from './components/FooterComponent.vue';


  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
      ShopComponent,
      JumboFooter,
      BottomFooter,
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