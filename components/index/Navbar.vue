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
    document.getElementById('navbar').style.top = - document.getElementById('navbar').clientHeight + 'px'
    window.onscroll = function () {
      if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
        document.getElementById('navbar').style.top = "0"
      } else {
        document.getElementById('navbar').style.top = - document.getElementById('navbar').clientHeight + 'px'
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
  transition: top 0.4s
  z-index: 2
  width: 100%
  background: white
  color: $primary
  &_logo
    font-weight: bold
    font-size: 2em
  &_links
    display: flex
    a
      cursor: pointer
      padding: 0 1em
      font-size: 1.4em
      transition: all 0.4s
    a:hover
@media only screen and (min-width: 992px)
  .navbar
    font-size: 15px  
    &_logo
      font-size: 3em

</style>
