<template lang="pug">
  #main
    .wrapper
      header header
      main main
      section section
      aside aside
      nav nav
      footer footer

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
    grid-auto-rows minmax(100px auto)
    grid-gap 10px
    grid-template-areas 'header header header header'\ 
                        'aside . main main'\ 
                        'nav nav main main'\ 
                        'section section section .'\ 
                        'footer footer footer footer'
    *
      background #eee
      padding 30px
      &:nth-child(even)
        background #ddd
        
    header 
      grid-area header
    main 
      grid-area main
    section 
      grid-area section
    aside 
      grid-area aside
    nav 
      grid-area nav
    footer 
      grid-area footer

</style>