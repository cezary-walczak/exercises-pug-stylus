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
      transform translate(-200px, 200px) scale(1.2, 1.5) rotateZ(-60deg)    
    
</style>