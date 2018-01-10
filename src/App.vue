<template lang="pug">
  #main
    .wrapper
      img(src='./assets/logo.png')

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="stylus">
  .wrapper
    width 100%
    padding 20px
    box-sizing border-box
    text-align center
    img
      position absolute
      top 100px
      animation animationer 3s 2s ease-in-out infinite alternate-reverse

@keyframes animationer
  from 
    transform translateX(-100px)
  to
    transform translateX(100px)

</style>