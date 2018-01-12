<template lang="pug">
  #main
    .wrapper
      header
        img(src='./assets/logo.png')

      form
        p You are a...
        input#male(type='radio' name='gender')
        label(for='male') male
        br
        input#female(type='radio' name='gender')
        label(for='female') female

        p ...who is interested in...
        input#web(type='checkbox')
        label(for='web') web development
        br
        input#photoshop(type='checkbox')
        label(for='photoshop') photoshop
        br
        input#another(type='checkbox')
        label(for='another') doing weird things

        p contact details
        fieldset 
          legend contact-info
          input(
            type='email' 
            placeholder='email' 
            required
          )
          span.tick
          input(
            type='telephone' 
            placeholder='phone number' 
            required
          )
          span.tick

        p how would you like to contact?
        select
          option by email
          option by telephone
        input(type='submit' value='become a ninja')

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
  dp = 20px

  hideInput() 
    opacity 0 
    width 0 
    margin 0 
  
  labelStyle()
    margin-bottom 10px
    display inline-block
    padding-left dp
    line-height 1.2rem
    cursor pointer

  #main
    background #eee
    margin 0
    font-family arial
    .wrapper
      header
        background #ccc
        padding dp
        text-align center

      form
        padding dp
        p
          font-size 2rem
          letter-spacing 0.2rem
        input[type=radio]
          hideInput()
          &:checked + label[for=male]
          &:checked + label[for=female]
            background-position 0 0
            color #42b883
        label[for=male]
        label[for=female]
          labelStyle()
          background url(./assets/checks.png) no-repeat 0 -33px

        input[type=checkbox]
          hideInput()
          &:checked + label[for=web]
          &:checked + label[for=photoshop]
          &:checked + label[for=another]
            background-position 0 -66px
            color #42b883
        label[for=web]
        label[for=photoshop]
        label[for=another]
          labelStyle()
          background url(./assets/checks.png) no-repeat 0 -99px

</style>