<template>
  <div class="row">
    <SingleCard v-for="card in AppMain" :key="card"/>
  </div>
</template>

<script>
import SingleCard from './SingleCard.vue';

export default {
    name: 'AppMain',
    components: {
    SingleCard
    },

    data(){
        return{
            AppMain: [],
            endpoint: 'https://flynn.boolean.careers/exercises/api/array/music'
        }
    }
}

</script>

<style lang="scss">


</style>