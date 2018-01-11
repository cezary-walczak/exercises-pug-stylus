<template lang="pug">
  #main
    .wrapper
      .flex-container
        .box.one
        .box.two
        .box.three

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
    .flex-container
      display flex
      flex-wrap wrap
      justify-content space-between
      .box
        height 100px
        flex-basis 100px
        &.one
          background red
          order 0
        &.two
          background blue
          order 2
        &.three
          background green
          order -2

</style>