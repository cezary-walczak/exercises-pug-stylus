<template lang="pug">
  #main
    .wrapper
      img(src='./assets/logo.png' )
      p.
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
        Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
        Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!

      .box.blue
      .box.red
      .box.green

      .service
        h2 Service 1
        p This is service 1
      .service
        h2 Service 2
        p This is service 2
      .service
        h2 Service 3
        p This is service 3

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
    background #eee
    max-width 960px
    margin 0 auto
    padding 20px
    &:after
      content ""
      display block
      clear both
    img
      float right
      margin 10px

    .box
      width: 100px
      height 100px
    .blue
      background blue
      float right
    .red
      background red
      float left
    .green
      background green
      margin auto

    .service
      float left
      background #ddd
      width 29%
      margin 1%
      padding 1%
      text-align center
      h1, p
        color #999
        margin 10px 0
        text-align center

</style>