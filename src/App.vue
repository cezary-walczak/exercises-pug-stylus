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
    grid-template-columns repeat(6, 1fr)
    grid-template-rows repeat(4, minmax(150px, auto))
    grid-gap 10px
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
      &.div1
        // grid-column-start 1
        // grid-column-end 3 
        grid-column 1/3
      &.div2
        grid-column 3/7
      &.div3
        grid-column 1/4
        grid-row 2/4
      &.div4
        grid-column 4/7
        grid-row 2/4
      &.div5
        grid-column 3/7
      &.div6
        grid-row 4
        grid-column 1/3
</style>