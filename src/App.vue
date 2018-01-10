<template lang="pug">
  #main
    p test
    p test
    a(href='') test
    a(href='') test
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
  p, a
    width 20%
    margin 20px
    padding 30px
    border 2px solid #000
    display inline-block
</style>