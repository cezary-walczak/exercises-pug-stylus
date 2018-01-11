<template lang="pug">
  #main
    .wrapper
      nav
        ul
          li
            a(href='') menu-item-1
          li
            a(href='') menu-item-2
          li
            a(href='') menu-item-3
          li
            a(href='') menu-item-4

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

min-screen = 30em

  .wrapper
    width 100%
    nav 
      background #333
      ul
        list-style-type none 
        padding 0

        li
          a
            text-decoration none 
            text-align center
            color #fff
            display block
            padding 10px
            background #666
            &:hover
              background #999

    .flex-container
      display flex
      flex-wrap wrap
      .box
        height 100px
        flex 1 0 400px
        &.one
          background red
        &.two
          background blue
        &.three
          background green

@media screen and (min-width min-screen)
  nav
    ul
      display flex
      justify-content space-around
      li
        flex 1 1 0

</style>