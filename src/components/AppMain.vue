<template>
  <div class="row row-cols-5">
    <SingleCard v-for="info in infolist" :key="info.id" :info="info"/>

  </div>
</template>

<script>
import axios from 'axios';
import SingleCard from './SingleCard.vue';

export default {
    name: 'AppMain',
    components: {
    SingleCard,
},
    
    data(){
        return{
            infolist: [],
        }
    },
    
    created() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
          this.infolist = response.data.response;
        })
        .catch((err) => {
          console.log(err);
        })
    }
}

</script>

<style lang="scss">


</style>