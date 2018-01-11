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

      .change-layout
        a(
          href='#' 
          v-on:click='stackLayout = !stackLayout'
        ) change layout

      section
        article(v-bind:class='{ stack: stackLayout }')
          h2 header-1
          p.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Magni blanditiis consectetur laboriosam rerum, eos dolor perspiciatis atque amet reprehenderit, 
            aperiam numquam vel voluptatem sunt. Reprehenderit voluptate quidem eveniet debitis natus.
        article(v-bind:class='{ stack: stackLayout }')
          h2 header-2
          p.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Magni blanditiis consectetur laboriosam rerum, eos dolor perspiciatis atque amet reprehenderit, 
            aperiam numquam vel voluptatem sunt. Reprehenderit voluptate quidem eveniet debitis natus.
        article(v-bind:class='{ stack: stackLayout }')
          h2 header-3
          p.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Magni blanditiis consectetur laboriosam rerum, eos dolor perspiciatis atque amet reprehenderit, 
            aperiam numquam vel voluptatem sunt. Reprehenderit voluptate quidem eveniet debitis natus.
        article(v-bind:class='{ stack: stackLayout }')
          h2 header-4
          p.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Magni blanditiis consectetur laboriosam rerum, eos dolor perspiciatis atque amet reprehenderit, 
            aperiam numquam vel voluptatem sunt. Reprehenderit voluptate quidem eveniet debitis natus.
        

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      stackLayout: true
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

    .change-layout
      a
        padding 10px
        margin: 20px 

    section 
      margin 20px
      article
        background #eee
        margin-bottom 20px
        padding 10px
        box-sizing border-box
        h2, p
          text-align center
          margin 10 0

@media screen and (min-width min-screen)
  nav
    display flex
    justify-content space-between
    ul
      display flex
      li
        flex 1 1 0

  section 
    display flex
    flex-wrap wrap
    justify-content space-between
    article
      flex 0 1 30%
      transition flex-basis 0.3s ease
      &.stack {
        flex 0 1 100%
      }

</style>