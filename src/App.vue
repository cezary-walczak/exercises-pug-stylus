<template lang="pug">
  #main
    .wrapper
      div 1
      div 2
      div 3
      div 4
      div 5
      div 6
      div 7
      div 8
      div 9

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
    // grid-template-columns 30% 20% 50%
    // grid-template-columns 1fr 2fr 1fr
    grid-template-columns repeat(3, 1fr)
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd

</style>