<template>
  <div id="app">

    <AppHeader/>
    <AppMain/>

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
}
}
</script>

<style lang="scss">

@import '@/style/generic.scss'



</style>
