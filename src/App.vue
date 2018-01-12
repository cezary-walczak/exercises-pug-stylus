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

</style>