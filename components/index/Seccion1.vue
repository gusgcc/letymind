<template>
  <div class="seccion1">
    <div class="seccion1_izq">
      <h1>
        Lorem ipsum dolor sit amet.
      </h1>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cum neque
        consectetur necessitatibus error.
      </p>
      <div class="container_buttons">
        <button>Try Dropbox Bussines</button>
        <button>Get Dropbox Basic</button>
      </div>
    </div>
    <div class="seccion1_der">
      <div class="img_container">
        <img
          width="100%"
          src="~/assets/index/img/foto.jpg"
          alt="Imagen"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="sass" scoped>
.seccion1
  width: 100%
  background: rgba(76,27,255,0.1)
  &_izq
    padding: 2em 4em
    h1, p
      width: 100%
      color: $primary
      margin-bottom: 1em
      font-size: 1.7em
    h1
      font-size: 4em
    .container_buttons
      display: flex
      flex-direction: row
      justify-content: space-around
      align-items: center
      width: 100%
      button
        overflow: none
        outline: none
        color: $primary
        font-weight: bold
        font-size: 1.8em
        width: 40%
        background: none
        border: 2px solid $primary
        padding: 1em 1em
        border-radius: 2em
        margin-bottom: 2em
        transition: all 0.4s
        cursor: pointer
      button:hover
        background: $primary
        color: white
    &_der
@media only screen and (min-width: 992px)
  .seccion1
    display: flex
    flex-direction: row
    &_izq
      display: flex
      flex-direction: column
      justify-content: center
      align-items: center
      width: 50%
    &_der
      width: 50%

</style>
