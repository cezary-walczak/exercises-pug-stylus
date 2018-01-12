<template lang="pug">
  #main
    input(type='checkbox' v-on:click='gridShow = !gridShow')

    .wrapper
      header header
      main main
      section section
      aside aside
      nav nav
      footer footer

      .grid(v-bind:class='{ showGrid: gridShow }')
        p
        p
        p
        p
        p
        p
        p
        p
        p
        p
        p
        p

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
    grid-template-columns repeat(12, 1fr)
    grid-auto-rows minmax(100px auto)
    grid-gap 10px
    position relative
    *
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
    header
      grid-column 1/13
    main
      grid-column 4/13
      grid-row 2/4
    section 
      grid-column 1/13
      grid-row 4/6
    aside
    nav
      grid-column 1/4
    footer
      grid-column 1/13

    .grid
      display grid
      position absolute
      left 0
      top 0
      grid-template-columns repeat(12, 1fr)
      grid-auto-rows minmax(100% auto)
      width 100%
      height 100%
      padding 0
      opacity 0.1
      display none
      p
        border 1px solid #666

    .showGrid
      display grid

</style>