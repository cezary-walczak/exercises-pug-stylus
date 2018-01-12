<template lang="pug">
  #main
    .wrapper
      .div1 1
      .div2 2
      .div3 3
      .div4 4
      .div5.nested
        p 1
        p 2
        p 3
        p 4
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
    grid-gap 10px
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
      &.nested
        display grid
        grid-template-columns 1fr 1fr
        grid-gap 10px
        grid-column span 3
        p
          border 1px solid #fff
          padding 10px
          margin 0
</style>