<template>
  <div class="header_style p-2 d-flex">
    <img src="../images/Spotify-Icon-Logo.wine.svg" alt="Logo Spotify">
    <SearchBar/>
  </div>
</template>

<script>
import SearchBar from './SearchBar.vue';

export default {
    name: 'AppHeader',

    components: {
      SearchBar
    },              

    data(){
      return{
        searchGen: ''
      }
    }
}
</script>

<style lang="scss">

.header_style{
    background-color: rgb(46, 58, 70);

    img{
        height: 60px;
    }
}

</style>