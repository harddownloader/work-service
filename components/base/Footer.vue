<template lang="pug">
//
  Footer
  ================================================== 
#footer
  // Footer Top Section
  .footer-top-section
    .container
      .row
        .col-xl-12
          // Footer Rows Container
          .footer-rows-container
            // Left Side
            .footer-rows-left
              .footer-row
                .footer-row-inner.footer-logo
                  img(src='images/logo2.png', alt='')
            // Right Side
            .footer-rows-right
              // Social Icons
              .footer-row
                .footer-row-inner
                  ul.footer-social-links
                    li
                      a(href='#', title='Facebook', data-tippy-placement='bottom', data-tippy-theme='light')
                        i.icon-brand-facebook-f
                    li
                      a(href='#', title='Twitter', data-tippy-placement='bottom', data-tippy-theme='light')
                        i.icon-brand-twitter
                    li
                      a(href='#', title='Google Plus', data-tippy-placement='bottom', data-tippy-theme='light')
                        i.icon-brand-google-plus-g
                    li
                      a(href='#', title='LinkedIn', data-tippy-placement='bottom', data-tippy-theme='light')
                        i.icon-brand-linkedin-in
                  .clearfix
              // Language Switcher
              .footer-row
                .footer-row-inner
                multiselect.selectpicker.language-switcher(
                  v-model="value_lang",
                  :options="options_lang",
                  :searchable="false",
                  :close-on-select="false",
                  :show-labels="false"
                  placeholder="Русский"
                )
                  //select.selectpicker.language-switcher(data-selected-text-format='count', data-size='5')
                    option(selected='') English
                    option Français
                    option Español
                    option Deutsch
          // Footer Rows Container / End
          // Footer Top Section / End
          // Footer Middle Section
          .footer-middle-section
            .container
              .row
                // Links
                .col-xl-2.col-lg-2.col-md-3
                  .footer-links
                    h3 For Candidates
                    ul
                      li
                        a(href='#')
                          span Browse Jobs
                      li
                        a(href='#')
                          span Add Resume
                      li
                        a(href='#')
                          span Job Alerts
                      li
                        a(href='#')
                          span My Bookmarks
                // Links
                .col-xl-2.col-lg-2.col-md-3
                  .footer-links
                    h3 For Employers
                    ul
                      li
                        a(href='#')
                          span Browse Candidates
                      li
                        a(href='#')
                          span Post a Job
                      li
                        a(href='#')
                          span Post a Task
                      li
                        a(href='#')
                          span Plans & Pricing
                // Links
                .col-xl-2.col-lg-2.col-md-3
                  .footer-links
                    h3 Helpful Links
                    ul
                      li
                        a(href='#')
                          span Contact
                      li
                        a(href='#')
                          span Privacy Policy
                      li
                        a(href='#')
                          span Terms of Use
                // Links
                .col-xl-2.col-lg-2.col-md-3
                  .footer-links
                    h3 Account
                    ul
                      li
                        a(href='#')
                          span Log In
                      li
                        a(href='#')
                          span My Account
                // Newsletter
                .col-xl-4.col-lg-4.col-md-12
                  h3
                    i.icon-feather-mail
                    |  Sign Up For a Newsletter
                  p Weekly breaking news, analysis and cutting edge advices on job searching.
                  form.newsletter(action='#', method='get')
                    input(type='text', name='fname', placeholder='Enter your email address')
                    button(type='submit')
                      i.icon-feather-arrow-right
          // Footer Middle Section / End
          // Footer Copyrights
          .footer-bottom-section
            .container
              .row
                .col-xl-12
                  | © 2019 
                  strong Hireo
                  | . All Rights Reserved.
          // Footer Copyrights / End
// Footer / End

</template>

<script>
import Multiselect from 'vue-multiselect'

export default {
  components: { Multiselect },
  data () {
    return {
      value_lang: null,
      options_lang: [
        "Русский",
        "Украинский",
      ],

    }
  }
}
</script>

<style scoped>

</style>