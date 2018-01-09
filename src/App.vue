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
  lightGray = #eee
  red = #be2525

  border-radius(radius = 10px)
    -webkit-border-radius radius
    border-radius radius

  clear-fix()
    zoom 1
    &:after
    &:before
      content ""
      display table
    &:after
      clear both

  section
    width 200px
    height 200px
    background lightGray
    color red
    border solid 1px @color
    div
      width 100px
      height 100px
      border solid 1px @color
      border-radius 30px
      clear-fix()

</style>