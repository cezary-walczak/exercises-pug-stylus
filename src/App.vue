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
      background #eee
      display flex
      flex-wrap wrap
      flex-flow column-reverse
      justify-content center
      height 800px
      .box
        height 100px
        flex 0 0 100px
        &.one
          background red
        &.two
          background blue
        &.three
          background green

</style>