<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
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