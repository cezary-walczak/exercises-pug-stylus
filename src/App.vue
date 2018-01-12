<template lang="pug">
  #main
    .wrapper
      div 1
      div 2
      div 3
      div 4
      div Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam ea rem consectetur saepe accusantium est expedita doloremque suscipit ut quidem, illum architecto facilis. Illum quia quidem architecto repellendus? Deleniti, incidunt. Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam ea rem consectetur saepe accusantium est expedita doloremque suscipit ut quidem, illum architecto facilis. Illum quia quidem architecto repellendus? Deleniti, incidunt.Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam ea rem consectetur saepe accusantium est expedita doloremque suscipit ut quidem, illum architecto facilis. Illum quia quidem architecto repellendus? Deleniti, incidunt.
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
    // grid-auto-rows minmax(200px, auto)
    // grid-template-rows 100px 200px 300px
    grid-template-rows repeat(3, minmax(200px, auto))
    // grid-column-gap 10px
    // grid-row-gap 10px
    grid-gap 10px
    div
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd

</style>