<template lang="pug">
//
  Page Content
  ================================================== 
.full-page-container.with-map
  .full-page-sidebar.hidden-sidebar
    .full-page-sidebar-inner(data-simplebar='')
      .sidebar-container
        // Keywords
        .sidebar-widget
          h3 Keywords
          .keywords-container
            .keyword-input-container
              input.keyword-input(type='text', placeholder='e.g. job title')
              button.keyword-input-button.ripple-effect
                i.icon-material-outline-add
            .keywords-list
              // keywords go here
            .clearfix
        // Category
        .sidebar-widget
          h3 Category
          select.selectpicker.default(multiple='', data-selected-text-format='count', data-size='7', title='All Categories')
            option Admin Support
            option Customer Service
            option Data Analytics
            option Design & Creative
            option Legal
            option Software Developing
            option IT & Networking
            option Writing
            option Translation
            option Sales & Marketing
        // Job Types
        .sidebar-widget
          h3 Job Type
          .switches-list
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                |  Freelance
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                |  Full Time
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                |  Part Time
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                |  Internship
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                |  Temporary
        // Salary
        .sidebar-widget
          h3 Salary
          .margin-top-55
          // Range Slider
          input.range-slider(type='text', value='', data-slider-currency='$', data-slider-min='1500', data-slider-max='15000', data-slider-step='100', data-slider-value='[1500,15000]')
        // Tags
        .sidebar-widget
          h3 Tags
          .tags-container
            .tag
              input#tag1(type='checkbox')
              label(for='tag1') front-end dev
            .tag
              input#tag2(type='checkbox')
              label(for='tag2') angular
            .tag
              input#tag3(type='checkbox')
              label(for='tag3') react
            .tag
              input#tag4(type='checkbox')
              label(for='tag4') vue js
            .tag
              input#tag5(type='checkbox')
              label(for='tag5') web apps
            .tag
              input#tag6(type='checkbox')
              label(for='tag6') design
            .tag
              input#tag7(type='checkbox')
              label(for='tag7') wordpress
          .clearfix
      // Sidebar Container / End
      // Search Button
      .sidebar-search-button-container
        button.button.ripple-effect Search
      // Search Button / End
      // Full Page Sidebar / End
      // Full Page Content
      .full-page-content-container(data-simplebar='')
        .full-page-content-inner
          h3.page-title Search Results
          .notify-box.margin-top-15
            .switch-container
              label.switch
                input(type='checkbox')
                span.switch-button
                span.switch-text Turn on email alerts for this search
            .sort-by
              span Sort by:
              select.selectpicker.hide-tick
                option Relevance
                option Newest
                option Oldest
                option Random
          .listings-container.grid-layout.margin-top-35
            // Job Listing
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-01.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company
                    | Hexagon 
                    span.verified-badge(title='Verified Employer', data-tippy-placement='top')
                  h3.job-listing-title Bilingual Event Support Specialist
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-05.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Laxo
                  h3.job-listing-title Competition Law Officer
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-02.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Coffee
                  h3.job-listing-title Barista and Cashier
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-03.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company
                    | King 
                    span.verified-badge(title='Verified Employer', data-tippy-placement='top')
                  h3.job-listing-title Restaurant General Manager
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-05.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Skyist
                  h3.job-listing-title International Marketing Coordinator
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-05.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Podous
                  h3.job-listing-title Construction Labourers
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-04.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Mates
                  h3.job-listing-title Administrative Assistant
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-06.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Trideo
                  h3.job-listing-title Human Resources Consultant
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-06.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Trideo
                  h3.job-listing-title International Marketing Specialist
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-02.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Coffee
                  h3.job-listing-title Terrain Cafe Barista
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-05.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Kinte
                  h3.job-listing-title Skilled Labourer
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Logo
                .job-listing-company-logo
                  img(src='images/company-logo-05.png', alt='')
                // Details
                .job-listing-description
                  h4.job-listing-company Alilia
                  h3.job-listing-title Healthcare Claims Advisor
              // Job Listing Footer
              .job-listing-footer
                span.bookmark-icon
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
          // Pagination
          .clearfix
          .pagination-container.margin-top-20.margin-bottom-20
            nav.pagination
              ul
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-left
                li
                  a.ripple-effect(href='#') 1
                li
                  a.ripple-effect.current-page(href='#') 2
                li
                  a.ripple-effect(href='#') 3
                li
                  a.ripple-effect(href='#') 4
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-right
          .clearfix
          // Pagination / End
          // Footer
          .small-footer.margin-top-15
            .small-footer-copyrights
              | © 2019 
              strong Hireo
              | . All Rights Reserved.
            ul.footer-social-links
              li
                a(href='#', title='Facebook', data-tippy-placement='top')
                  i.icon-brand-facebook-f
              li
                a(href='#', title='Twitter', data-tippy-placement='top')
                  i.icon-brand-twitter
              li
                a(href='#', title='Google Plus', data-tippy-placement='top')
                  i.icon-brand-google-plus-g
              li
                a(href='#', title='LinkedIn', data-tippy-placement='top')
                  i.icon-brand-linkedin-in
            .clearfix
          // Footer / End
          // Full Page Content / End
          // Full Page Map
          .full-page-map-container
            // Enable Filters Button
            .filter-button-container
              button.enable-filters-button
                i.enable-filters-button-icon
                span.show-text Show Filters
                span.hide-text Hide Filters
              .filter-button-tooltip Click to expand sidebar with filters!
            // Map
            #map(data-map-zoom='12', data-map-scroll='true')
          // Full Page Map / End

</template>

<script>

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