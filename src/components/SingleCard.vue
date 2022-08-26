<template>
  <div class="container my-5 style_main">
    <div class="card text-center" style="width: 18rem;">
        <img src="" class="card-img-top" alt="...">
        <div class="card-body">
            <p class="card-text">{{card.title}}</p>
            <p class="card-text">autore</p>
            <p class="card-text">anno</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'SingleCard',
    props: {
        card: Object
    }
}
</script>

<style lang="scss">
.style_main{
    background-color: rgb(30, 45, 59);

    .card{
        background-color: rgb(46, 58, 70);
    }
}
</style>