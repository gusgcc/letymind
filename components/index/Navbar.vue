<template>
  <ul
    id="navbar"
    class="navbar"
  >
    <li class="navbar_logo">
      <a>Link 1</a>
    </li>
    <div class="navbar_links">
      <a>Home</a>
      <a>Nosotros</a>
      <a>Aplica ahora</a>
    </div>
  </ul>
</template>

<script>
export default {
  mounted () {
    console.dir(document.getElementById('navbar').clientHeight, document.getElementById('navbar').offsetHeight, document.getElementById('navbar'))

    window.onscroll = function () {
      if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
        document.getElementById('navbar').style.top = "0"

      } else {
        document.getElementById('navbar').style.top = "-50px"
      }
    }
  }
};
</script>

<style lang="sass" scoped>
.navbar
  padding: 0 5%
  list-style: none
  display: flex
  justify-content: space-between
  align-items: center
  position: fixed
  top: -50px
  transition: top 0.4s
  z-index: 2
  width: 100%
  background: white
  &_logo
    font-weight: bold
    font-size: 2em
  &_links
    display: flex
    a
      padding: 0 1em
      font-size: 1.4em
@media only screen and (min-width: 992px)
  .navbar
    font-size: 15px  
    &_logo
      font-size: 3em

</style>
