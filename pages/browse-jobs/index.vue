<template lang="pug">
//
  Page Content
  ================================================== 
.container
  .row
    .col-xl-3.col-lg-4
      .sidebar-container
        // Location
        .sidebar-widget
          h3 Location
          .input-with-icon
            #autocomplete-container
              input#autocomplete-input(type='text', placeholder='Location')
            i.icon-material-outline-location-on
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
    .col-xl-9.col-lg-8.content-left-offset
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
      .listings-container.margin-top-35
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
              p.job-listing-text
                | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value.
            // Bookmark
            span.bookmark-icon
          // Job Listing Footer
          .job-listing-footer
            ul
              li
                i.icon-material-outline-location-on
                |  San Francissco
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
              p.job-listing-text
                | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value.
            // Bookmark
            span.bookmark-icon
          // Job Listing Footer
          .job-listing-footer
            ul
              li
                i.icon-material-outline-location-on
                |  San Francissco
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
              p.job-listing-text
                | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value.
            // Bookmark
            span.bookmark-icon
          // Job Listing Footer
          .job-listing-footer
            ul
              li
                i.icon-material-outline-location-on
                |  San Francissco
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
              p.job-listing-text
                | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value.
            // Bookmark
            span.bookmark-icon
          // Job Listing Footer
          .job-listing-footer
            ul
              li
                i.icon-material-outline-location-on
                |  San Francissco
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
        .row
          .col-md-12
            // Pagination
            .pagination-container.margin-top-30.margin-bottom-60
              nav.pagination
                ul
                  li.pagination-arrow
                    a(href='#')
                      i.icon-material-outline-keyboard-arrow-left
                  li
                    a(href='#') 1
                  li
                    a.current-page(href='#') 2
                  li
                    a(href='#') 3
                  li
                    a(href='#') 4
                  li.pagination-arrow
                    a(href='#')
                      i.icon-material-outline-keyboard-arrow-right
        // Pagination / End

</template>

<script>
  export default {
    layout: 'Simple',
    data: function () {
      return {
        
      }
    }
  }
</script>

<style lang="stylus" scoped>

</style>