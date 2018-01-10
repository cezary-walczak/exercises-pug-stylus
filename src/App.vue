<template lang="pug">
  #main
    .wrapper
      img(src='./assets/logo.png')
      button Hover me

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
      transform translate(-200px, 200px) scale(1.2, 1.5) rotateZ(-60deg)
    button
      width 100px
      height 100px
      border-radius 50px
      margin auto
      cursor pointer
      transition background 1s, transform 2s 1s ease
      &:hover
        background #42b883
        transform rotate(360deg)

</style>