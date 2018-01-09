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

  section
    width 200px
    height 200px
    background lightGray
    color red
    border solid 10px @color
    div
      width 100px
      height 100px
      border solid 10px @color

</style>