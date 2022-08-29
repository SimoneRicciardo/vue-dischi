<template>
  <div class="container my-5 style_main">
    <div class="card text-center card-style">
        <img :src="info.poster" class="card-img-top" :alt="info.author">
        <div class="card-body style_card text-light">
            <p>{{info.title}}</p>
            <p>{{info.author}}</p>
            <p>{{info.year}}</p>
        </div>
    </div>
  </div>
</template>

<script>

export default {
    name: 'SingleCard',
    props: {
        info: Object,
    }
}
</script>

<style lang="scss">
.style_main{
    background-color: rgb(30, 45, 59);

    .card{
        background-color: rgb(46, 58, 70);
            img{
                height: 200px;
            }
            .style_card{
                height: 150px;
            }
    }
}
</style>