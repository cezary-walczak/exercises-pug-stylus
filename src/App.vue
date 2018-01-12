<template lang="pug">
  #main
    .wrapper
      .div1 1
      .div2 2
      .div3 3
      .div4 4
      .div5 5

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      gridShow: false
    }
  }
}
</script>

<style lang="stylus">
  .wrapper
    max-width 960px
    margin 0 auto
    display grid
    grid-template-columns repeat(6, 1fr)
    grid-auto-rows minmax(150px, auto)
    grid-gap 10px
    position relative
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
      &.div1
        grid-column 1/3
        grid-row 1/5
      &.div2
        grid-column 3/7
        grid-row 1/3
      &.div3
        grid-column 3/5
        grid-row 3/5
      &.div4
        grid-column 5/7
        grid-row 3/7
      &.div5
        grid-column 1/5
        grid-row 5/7

</style>