<template lang="pug">
  #main
    .wrapper
      .services
        .service
          h2 Service 1
          p This is service 1
        .service
          h2 Service 2
          p This is service 2
        .service
          h2 Service 3
          p This is service 3
      .content
        h2 content
        p.
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
          Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
          Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!

      .columns
        section
          h2 this is column 1
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
        aside
          h2 this is column 1
          p.
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
            Consequatur inventore omnis soluta voluptates, enim magnam quis a ullam. 
            Reiciendis dolor laboriosam velit aperiam deserunt distinctio impedit ad commodi sapiente aliquid!
          img(src='./assets/logo.png')
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
  clear()
    &:after
      content ""
      display block
      clear both

  .wrapper
    background #eee
    max-width 960px
    margin 0 auto
    padding 20px
    clear()

    .services
      clear()
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

    .content
      padding 10px
      background #ccc
      clear both
      margin-top 100px

    .columns
      clear()
      section, aside
        float left
        width 46%
        padding 1%
        margin 1%
        background #bbb
</style>