<template lang="pug">
//
  Page Content
  ================================================== 
.container
  .row
    .col-xl-5.offset-xl-3
      .login-register-page
        // Welcome Text
        .welcome-text
          h3(style='font-size: 26px;') Let's create your account!
          span
            | Already have an account? 
            a(href='pages-login.html') Log In!
        // Account Type
        .account-type
          div
            input#freelancer-radio.account-type-radio(type='radio', name='account-type-radio', checked='')
            label.ripple-effect-dark(for='freelancer-radio')
              i.icon-material-outline-account-circle
              |  Freelancer
          div
            input#employer-radio.account-type-radio(type='radio', name='account-type-radio')
            label.ripple-effect-dark(for='employer-radio')
              i.icon-material-outline-business-center
              |  Employer
        // Form
        form#register-account-form(method='post')
          .input-with-icon-left
            i.icon-material-baseline-mail-outline
            input#emailaddress-register.input-text.with-border(type='text', name='emailaddress-register', placeholder='Email Address', required='')
          .input-with-icon-left(title='Should be at least 8 characters long', data-tippy-placement='bottom')
            i.icon-material-outline-lock
            input#password-register.input-text.with-border(type='password', name='password-register', placeholder='Password', required='')
          .input-with-icon-left
            i.icon-material-outline-lock
            input#password-repeat-register.input-text.with-border(type='password', name='password-repeat-register', placeholder='Repeat Password', required='')
        // Button
        button.button.full-width.button-sliding-icon.ripple-effect.margin-top-10(type='submit', form='login-form')
          | Register 
          i.icon-material-outline-arrow-right-alt
        // Social Login
        .social-login-separator
          span or
        .social-login-buttons
          button.facebook-login.ripple-effect
            i.icon-brand-facebook-f
            |  Register via Facebook
          button.google-login.ripple-effect
            i.icon-brand-google-plus-g
            |  Register via Google+

</template>

<script>
// titlebar
// page content(this)
// spacer
  export default {
    layout: 'Simple',
    components: {

    },
    methods: {

    },
    mutations: {

    },
    data: function () {
      return {
        
      }
    },
    
  }
</script>

<style lang="stylus" scoped>

</style>