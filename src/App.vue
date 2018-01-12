<template lang="pug">
  #main
    .wrapper
      .div1 1
      .div2 2
      .div3 3
      .div4 4
      .div5 5
      .div6 6

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
    max-width 960px
    margin 0 auto
    display grid
    grid-template-columns repeat(3, 1fr)
    grid-auto-rows (minmax(150px, auto))
    grid-gap 10px
    // align-items start
    justify-items streth
    align-items streth
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
      &.div5
        justify-self center
        align-self center
</style>