<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  .single-page-header(data-background-image='/images/single-job.jpg')
    .container
      .row
        .col-md-12
          .single-page-header-inner
            .left-side
              .header-image
                a(href='single-company-profile.html')
                  img(src='/images/company-logo-03a.png', alt='')
              .header-details
                h3 Restaurant General Manager
                h5 About the Employer
                ul
                  li
                    a(href='single-company-profile.html')
                      i.icon-material-outline-business
                      |  King
                  li
                    .star-rating(data-rating='4.9')
                  li
                    img.flag(src='/images/flags/gb.svg', alt='')
                    |  United Kingdom
                  li
                    .verified-badge-with-title Verified
            .right-side
              .salary-box
                .salary-type Annual Salary
                .salary-amount $35k - $38k

  //
    Page Content
    ================================================== 
  .container
    .row
      // Content
      .col-xl-8.col-lg-8.content-right-offset
        .single-page-section
          h3.margin-bottom-25 Job Description
          p
            | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
          p
            | Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.
          p
            | Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.
        .single-page-section
          h3.margin-bottom-30 Location
          #single-job-map-container
            #singleListingMap(data-latitude='51.507717', data-longitude='-0.131095', data-map-icon='im im-icon-Hamburger')
            a#streetView(href='#') Street View
        .single-page-section
          h3.margin-bottom-25 Similar Jobs
          // Listings Container
          .listings-container.grid-layout
            // Job Listing
            a.job-listing(href='#')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='/images/company-logo-02.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Coffee
                  h3.job-listing-title Barista and Cashier
              // Job Listing Footer
              .job-listing-footer
                ul
                  li
                    i.icon-material-outline-location-on
                    |  San Francisco
                  li
                    i.icon-material-outline-business-center
                    |  Full Time
                  li
                    i.icon-material-outline-account-balance-wallet
                    |  $35000-$38000
                  li
                    i.icon-material-outline-access-time
                    |  2 days ago
            // Job Listing
            a.job-listing(href='#')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='/images/company-logo-03.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company
                    | King 
                    span.verified-badge(title='Verified Employer', data-tippy-placement='top')
                  h3.job-listing-title Restaurant Manager
              // Job Listing Footer
              .job-listing-footer
                ul
                  li
                    i.icon-material-outline-location-on
                    |  San Francisco
                  li
                    i.icon-material-outline-business-center
                    |  Full Time
                  li
                    i.icon-material-outline-account-balance-wallet
                    |  $35000-$38000
                  li
                    i.icon-material-outline-access-time
                    |  2 days ago
          // Listings Container / End
      // Sidebar
      .col-xl-4.col-lg-4
        .sidebar-container
          a.apply-now-button.popup-with-zoom-anim(href='#small-dialog')
            | Apply Now 
            i.icon-material-outline-arrow-right-alt
          // Sidebar Widget
          .sidebar-widget
            .job-overview
              .job-overview-headline Job Summary
              .job-overview-inner
                ul
                  li
                    i.icon-material-outline-location-on
                    span Location
                    h5 London, United Kingdom
                  li
                    i.icon-material-outline-business-center
                    span Job Type
                    h5 Full Time
                  li
                    i.icon-material-outline-local-atm
                    span Salary
                    h5 $35k - $38k
                  li
                    i.icon-material-outline-access-time
                    span Date Posted
                    h5 2 days ago
          // Sidebar Widget
          .sidebar-widget
                h3 Bookmark or Share
                // Bookmark Button
                button.bookmark-button.margin-bottom-25
                  span.bookmark-icon
                  span.bookmark-text Bookmark
                  span.bookmarked-text Bookmarked
                // Copy URL
                .copy-url
                  input#copy-url.with-border(type='text', value='')
                  button.copy-url-button.ripple-effect(data-clipboard-target='#copy-url', title='Copy to Clipboard', data-tippy-placement='top')
                    i.icon-material-outline-file-copy
                // Share Buttons
                .share-buttons.margin-top-25
                  .share-buttons-trigger
                    i.icon-feather-share-2
                  .share-buttons-content
                    span
                      | Interesting? 
                      strong Share It!
                    ul.share-buttons-icons
                      li
                        a(href='#', data-button-color='#3b5998', title='Share on Facebook', data-tippy-placement='top')
                          i.icon-brand-facebook-f
                      li
                        a(href='#', data-button-color='#1da1f2', title='Share on Twitter', data-tippy-placement='top')
                          i.icon-brand-twitter
                      li
                        a(href='#', data-button-color='#dd4b39', title='Share on Google Plus', data-tippy-placement='top')
                          i.icon-brand-google-plus-g
                      li
                        a(href='#', data-button-color='#0077b5', title='Share on LinkedIn', data-tippy-placement='top')
                          i.icon-brand-linkedin-in


</template>

<script>
// titlebar
import TitleBar from '~/components/base/TitleBar.vue'
// page content(this)
  export default {
    layout: 'Simple',
    components: {
      TitleBar
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