<template lang="pug">
  section
    div
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
  @import '*'

  section
    width 200px
    height 200px
    background lightGray
    color red
    border solid 1px @color
    margin-left: -10px
    div
      margin-left abs(@margin-left)
      background rgba(#fff, 0.9)
      background grayscale(blue)
      background desaturate(blue, 60%)
      margin-top abs(-10px)
      margin-top ceil(4.4%)
      margin-top unit(4.4%, 'px')
      width 100px
      height 100px
      border solid 1px @color
      border-radius 30px
      clear-fix()

</style>