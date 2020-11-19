<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  #titlebar.gradient
    .container
      .row
        .col-md-12
          h2 Log In
          // Breadcrumbs
          nav#breadcrumbs.dark
            ul
              li
                a(href='#') Home
              li Log In
  //
    Page Content
    ==================================================
  .container
    .row
      .col-xl-5.offset-xl-3
        .login-register-page
          // Welcome Text
          .welcome-text
            h3 We're glad to see you again!
            span
              | Don't have an account? 
              a(href='pages-register.html') Sign Up!
          // Form
          form#login-form(method='post')
            .input-with-icon-left
              i.icon-material-baseline-mail-outline
              input#emailaddress.input-text.with-border(type='text', name='emailaddress', placeholder='Email Address', required='')
            .input-with-icon-left
              i.icon-material-outline-lock
              input#password.input-text.with-border(type='password', name='password', placeholder='Password', required='')
            a.forgot-password(href='#') Forgot Password?
          // Button
          button.button.full-width.button-sliding-icon.ripple-effect.margin-top-10(type='submit', form='login-form')
            | Log In 
            i.icon-material-outline-arrow-right-alt
          // Social Login
          .social-login-separator
            span or
          .social-login-buttons
            button.facebook-login.ripple-effect
              i.icon-brand-facebook-f
              |  Log In via Facebook
            button.google-login.ripple-effect
              i.icon-brand-google-plus-g
              |  Log In via Google+
  // Spacer
  .margin-top-70
  // Spacer / End

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