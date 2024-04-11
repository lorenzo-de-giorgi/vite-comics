<template>
  <HeaderComponent />
  <MainComponent />
  <FooterTop />
  <FooterBottom />
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterTop from './components/FooterTop.vue'
  import FooterBottom from './components/FooterBottom.vue';
  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
      FooterTop,
      FooterBottom
    },
    data() {
      return {
        
      }
    },
  }
</script>

<style lang="scss" scoped>

</style>