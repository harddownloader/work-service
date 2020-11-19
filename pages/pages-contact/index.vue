<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  #titlebar.gradient
    .container
      .row
        .col-md-12
          h2 Contact
          // Breadcrumbs
          nav#breadcrumbs.dark
            ul
              li
                a(href='#') Home
              li
                a(href='#') Pages
              li Contact
  //
    Content
    ==================================================
  // Container
  .container
    .row
      .col-xl-12
        .contact-location-info.margin-bottom-50
          .contact-address
            ul
              li.contact-address-headline Our Office
              li 425 Berry Street, CA 93584
              li Phone (123) 123-456
              li
                a(href='#') mail@example.com
              li
                .freelancer-socials
                  ul
                    li
                      a(href='#', title='Dribbble', data-tippy-placement='top')
                        i.icon-brand-dribbble
                    li
                      a(href='#', title='Twitter', data-tippy-placement='top')
                        i.icon-brand-twitter
                    li
                      a(href='#', title='Behance', data-tippy-placement='top')
                        i.icon-brand-behance
                    li
                      a(href='#', title='GitHub', data-tippy-placement='top')
                        i.icon-brand-github
          #single-job-map-container
            #singleListingMap(data-latitude='37.777842', data-longitude='-122.391805', data-map-icon='im im-icon-Hamburger')
            a#streetView(href='#') Street View
      .col-xl-8.col-lg-8.offset-xl-2.offset-lg-2
        section#contact.margin-bottom-60
          h3.headline.margin-top-15.margin-bottom-35 Any questions? Feel free to contact us!
          form#contactform(method='post', name='contactform', autocomplete='on')
            .row
              .col-md-6
                .input-with-icon-left
                  input#name.with-border(name='name', type='text', placeholder='Your Name', required='required')
                  i.icon-material-outline-account-circle
              .col-md-6
                .input-with-icon-left
                  input#email.with-border(name='email', type='email', placeholder='Email Address', pattern='^[A-Za-z0-9](([_\.\-]?[a-zA-Z0-9]+)*)@([A-Za-z0-9]+)(([\.\-]?[a-zA-Z0-9]+)*)\.([A-Za-z]{2,})$', required='required')
                  i.icon-material-outline-email
            .input-with-icon-left
              input#subject.with-border(name='subject', type='text', placeholder='Subject', required='required')
              i.icon-material-outline-assignment
            div
              textarea#comments.with-border(name='comments', cols='40', rows='5', placeholder='Message', spellcheck='true', required='required')
            input#submit.submit.button.margin-top-15(type='submit', value='Submit Message')
  // Container / End

</template>

<script>
// titlebar
// container (this)
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