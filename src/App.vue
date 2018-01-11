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
      flex-wrap wrap-reverse
      .box
        height 100px
        min-width 300px
        flex-grow 1
        &.one
          background red
        &.two
          background blue
        &.three
          background green

</style>