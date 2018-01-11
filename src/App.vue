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
      .box
        height 100px
        flex-basis 800px
        &.one
          background red
        &.two
          background blue
        &.three
          background green

</style>