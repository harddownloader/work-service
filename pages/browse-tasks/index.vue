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
        // Keywords
        .sidebar-widget
          h3 Keywords
          .keywords-container
            .keyword-input-container
              input.keyword-input(type='text', placeholder='e.g. task title')
              button.keyword-input-button.ripple-effect
                i.icon-material-outline-add
            .keywords-list
              // keywords go here
            .clearfix
        // Budget
        .sidebar-widget
          h3 Fixed Price
          .margin-top-55
          // Range Slider
          input.range-slider(type='text', value='', data-slider-currency='$', data-slider-min='10', data-slider-max='2500', data-slider-step='25', data-slider-value='[10,2500]')
        // Hourly Rate
        .sidebar-widget
          h3 Hourly Rate
          .margin-top-55
          // Range Slider
          input.range-slider(type='text', value='', data-slider-currency='$', data-slider-min='10', data-slider-max='150', data-slider-step='5', data-slider-value='[10,200]')
        // Tags
        .sidebar-widget
          h3 Skills
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
          // More Skills
          .keywords-container.margin-top-20
            .keyword-input-container
              input.keyword-input(type='text', placeholder='add more skills')
              button.keyword-input-button.ripple-effect
                i.icon-material-outline-add
            .keywords-list
              // keywords go here
            .clearfix
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
      // Tasks Container
      .tasks-list-container.tasks-grid-layout.margin-top-35
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title Food Delviery Mobile App
              ul.task-icons
                li
                  i.icon-material-outline-location-on
                  |  San Francisco
                li
                  i.icon-material-outline-access-time
                  |  2 minutes ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $1,000 - $2,500
                span Fixed Price
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title 2000 Words English to German
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  5 minutes ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $75
                span Fixed Price
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title Fix Python Selenium Code
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  30 minutes ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $100 - $150
                span Hourly Rate
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title WordPress Theme Installation
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  1 hour ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $100
                span Fixed Price
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title PHP Core Website Fixes
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  1 hour ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $50 - $80
                span Hourly Rate
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title Adsense Expert
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  2 hours ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $70 - $100
                span Hourly Rate
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title Design a Landing Page
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  2 hours ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $500
                span Fixed Price
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
        // Task
        a.task-listing(href='single-task-page.html')
          // Job Listing Details
          .task-listing-details
            // Details
            .task-listing-description
              h3.task-listing-title Website and Logo Redesign
              ul.task-icons
                li
                  i.icon-material-outline-location-off
                  |  Online Job
                li
                  i.icon-material-outline-access-time
                  |  3 hours ago
          .task-listing-bid
            .task-listing-bid-inner
              .task-offers
                strong $850 - $1000
                span Fixed Price
              span.button.button-sliding-icon.ripple-effect
                | Bid Now 
                i.icon-material-outline-arrow-right-alt
      // Tasks Container / End
      // Pagination
      .clearfix
      .row
        .col-md-12
          // Pagination
          .pagination-container.margin-top-60.margin-bottom-60
            nav.pagination
              ul
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-left
                li
                  a.ripple-effect(href='#') 1
                li
                  a.current-page.ripple-effect(href='#') 2
                li
                  a.ripple-effect(href='#') 3
                li
                  a.ripple-effect(href='#') 4
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-right
      // Pagination / End

</template>

<script>
  export default {
    layout: 'Simple',
  }
</script>

<style scoped>

</style>