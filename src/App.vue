<template>
  <HeaderComponent />
  <MainComponent />
  <ShopComponent />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import ShopComponent from './components/ShopComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
      ShopComponent,
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