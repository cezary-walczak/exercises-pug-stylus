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
      .box
        height 100px
        width 300px
        &.one
          background red
          flex-shrink 2
        &.two
          background blue
          flex-shrink 3
        &.three
          background green
          flex-shrink 1

</style>