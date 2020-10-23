<template>
  <div class="seccion2">
    <h1>Do more with Dopbox Business</h1>
    <div class="seccion2_cards">
      <CardPrecio class="card"></CardPrecio>
      <CardPrecio class="card"></CardPrecio>
      <CardPrecio class="card"></CardPrecio>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="sass" scoped>
.seccion2
  padding: 3em 0
  h1
    text-align: center
    margin: 2em 0
  &_cards
    display: flex
    flex-direction: row
    justify-content: space-around
    .card
      width: 25%
      height: 500px
            
    
</style>