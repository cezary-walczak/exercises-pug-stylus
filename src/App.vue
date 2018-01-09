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
    margin-left: add(1px, 2px)
    div
      margin-left abs(@margin-left)
      margin marginer(10px, 20px)
      background rgba(#fff, 0.9)
      width 100px
      height 100px
      border solid 1px @color
      border-radius 30px
      clear-fix()
      transition(all 1s ease)

</style>