<template>
    <HeaderComponent />
    <MainComponent />
    <TopFooterComponent />
    <MiddleFooterComponent />
    <BottomFooterComponent />

</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import TopFooterComponent from './components/TopFooterComponent.vue'
import MiddleFooterComponent from './components/MiddleFooterComponent.vue'
import BottomFooterComponent from './components/BottomFooterComponent.vue'



  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent,
      TopFooterComponent,
      MiddleFooterComponent,
      BottomFooterComponent,
    }
  }
</script>

<style lang="scss" scoped>


</style>