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
        ul
          li
            a(href='').icon submenu-item-1
          li
            a(href='').icon submenu-item-2

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

min-screen = 800px

  .wrapper
    width 100%
    nav 
      background #333
      ul
        list-style-type none 
        padding 0
        margin 0
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
            &.icon
              background url('./assets/logo.png') no-repeat center center / contain
              color transparent
              text-indent -10000px

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
    display flex
    justify-content space-between
    ul
      display flex
      li
        flex 1 1 0

</style>