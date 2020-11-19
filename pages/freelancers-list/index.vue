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
        // Hourly Rate
        .sidebar-widget
          h3 Hourly Rate
          .margin-top-55
          // Range Slider
          input.range-slider(type='text', value='', data-slider-currency='$', data-slider-min='10', data-slider-max='250', data-slider-step='5', data-slider-value='[10,250]')
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
      // Freelancers List Container
      .freelancers-container.freelancers-list-layout.margin-top-35
        // Freelancer
        .freelancer
          // Overview
          .freelancer-overview
            .freelancer-overview-inner
              // Bookmark Icon
              span.bookmark-icon
              // Avatar
              .freelancer-avatar
                .verified-badge
                a(href='single-freelancer-profile.html')
                  img(src='images/user-avatar-big-01.jpg', alt='')
              // Name
              .freelancer-name
                h4
                  a(href='#')
                    | Tom Smith 
                    img.flag(src='images/flags/gb.svg', alt='', title='United Kingdom', data-tippy-placement='top')
                span UI/UX Designer
                // Rating
                .freelancer-rating
                  .star-rating(data-rating='4.9')
          // Details
          .freelancer-details
            .freelancer-details-list
              ul
                li
                  | Location 
                  strong
                    i.icon-material-outline-location-on
                    |  London
                li
                  | Rate 
                  strong $60 / hr
                li
                  | Job Success 
                  strong 95%
            a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
              | View Profile 
              i.icon-material-outline-arrow-right-alt
        // Freelancer / End
        // Freelancer
        .freelancer
          // Overview
          .freelancer-overview
            .freelancer-overview-inner
              // Bookmark Icon
              span.bookmark-icon
              // Avatar
              .freelancer-avatar
                .verified-badge
                a(href='single-freelancer-profile.html')
                  img(src='images/user-avatar-big-02.jpg', alt='')
              // Name
              .freelancer-name
                h4
                  a(href='#')
                    | David Peterson 
                    img.flag(src='images/flags/de.svg', alt='', title='Germany', data-tippy-placement='top')
                span iOS Expert + Node Dev
                // Rating
                .freelancer-rating
                  .star-rating(data-rating='4.2')
          // Details
          .freelancer-details
            .freelancer-details-list
              ul
                li
                  | Location 
                  strong
                    i.icon-material-outline-location-on
                    |  Berlin
                li
                  | Rate 
                  strong $40 / hr
                li
                  | Job Success 
                  strong 88%
            a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
              | View Profile 
              i.icon-material-outline-arrow-right-alt
        // Freelancer / End
        // Freelancer
        .freelancer
          // Overview
          .freelancer-overview
            .freelancer-overview-inner
              // Bookmark Icon
              span.bookmark-icon
              // Avatar
              .freelancer-avatar
                a(href='single-freelancer-profile.html')
                  img(src='images/user-avatar-placeholder.png', alt='')
              // Name
              .freelancer-name
                h4
                  a(href='#')
                    | Marcin Kowalski 
                    img.flag(src='images/flags/pl.svg', alt='', title='Poland', data-tippy-placement='top')
                span Front-End Developer
                // Rating
                span.company-not-rated.margin-bottom-5 Minimum of 3 votes required
          // Details
          .freelancer-details
            .freelancer-details-list
              ul
                li
                  | Location 
                  strong
                    i.icon-material-outline-location-on
                    |  Warsaw
                li
                  | Rate 
                  strong $50 / hr
                li
                  | Job Success 
                  strong 100%
            a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
              | View Profile 
              i.icon-material-outline-arrow-right-alt
        // Freelancer / End
        // Freelancer
        .freelancer
          // Overview
          .freelancer-overview
            .freelancer-overview-inner
              // Bookmark Icon
              span.bookmark-icon
              // Avatar
              .freelancer-avatar
                .verified-badge
                a(href='single-freelancer-profile.html')
                  img(src='images/user-avatar-big-03.jpg', alt='')
              // Name
              .freelancer-name
                h4
                  a(href='#')
                    | Sindy Forest 
                    img.flag(src='images/flags/au.svg', alt='', title='Australia', data-tippy-placement='top')
                span Magento Certified Developer
                // Rating
                .freelancer-rating
                  .star-rating(data-rating='5.0')
          // Details
          .freelancer-details
            .freelancer-details-list
              ul
                li
                  | Location 
                  strong
                    i.icon-material-outline-location-on
                    |  Brisbane
                li
                  | Rate 
                  strong $70 / hr
                li
                  | Job Success 
                  strong 100%
            a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
              | View Profile 
              i.icon-material-outline-arrow-right-alt
        // Freelancer / End
        // Tasks Container / End
        // Pagination
        .clearfix
        .row
          .col-md-12
            // Pagination
            .pagination-container.margin-top-40.margin-bottom-60
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