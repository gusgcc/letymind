<template>
  <div class="card_precio">
    <h1 class="title">Pro</h1>
    <h5 class="subtitle"> lorem lorem </h5>
    <p class="info">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum voluptatem sed nam, doloremque quaerat cum, voluptatum velit magni eveniet minus laborum recusandae fugit dolore? Voluptatem libero nesciunt similique distinctio quam?</p>
    <span class="price">S/8.25</span>
    <span class="price_info">lorem</span>
    <button class="btn_start">Get started</button>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="sass" scoped>
.card_precio
    font-size: 10px
    display: flex
    flex-direction: column
    justify-content: space-around
    align-items: center
    padding: 1em 2em
    .title
        color: $primary
        font-size: 5em
        margin-bottom: 0px
        line-height: 1
    .subtitle
        font-size: 1.5em
    .info
        text-align: center
        font-size: 1.4em
    .price
        font-size: 5em
        color: $primary
        &_info
            font-size: 1.5em
    .btn_start
        font-size: 2em
        background: white
        border: 2px solid $primary
        color: $primary
        width: 80%
        padding: 0.5em 1em
        transition: all 0.4s
    .btn_start:hover
        background: $primary
        opacity: 0.7
        color: white

    
</style>