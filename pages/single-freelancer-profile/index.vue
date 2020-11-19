<template lang="pug">
duv
  //
    Titlebar
    ================================================== 
  .single-page-header.freelancer-header(data-background-image='/images/single-freelancer.jpg')
    .container
      .row
        .col-md-12
          .single-page-header-inner
            .left-side
              .header-image.freelancer-avatar
                img(src='/images/user-avatar-big-02.jpg', alt='')
              .header-details
                h3
                  | David Peterson 
                  span iOS Expert + Node Dev
                ul
                  li
                    .star-rating(data-rating='5.0')
                  li
                    img.flag(src='/images/flags/de.svg', alt='')
                    |  Germany
                  li
                    .verified-badge-with-title Verified
  //
    Page Content
    ==================================================
  .container
    .row
      // Content
      .col-xl-8.col-lg-8.content-right-offset
        // Page Content
        .single-page-section
          h3.margin-bottom-25 About Me
          p
            | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
          p
            | Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.
        // Boxed List
        .boxed-list.margin-bottom-60
          .boxed-list-headline
            h3
              i.icon-material-outline-thumb-up
              |  Work History and Feedback
          ul.boxed-list-ul
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | Web, Database and API Developer 
                    span Rated as Freelancer
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  August 2019
                  .item-description
                    p
                      | Excellent programmer - fully carried out my project in a very professional manner.
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | WordPress Theme Installation 
                    span Rated as Freelancer
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  June 2019
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | Fix Python Selenium Code 
                    span Rated as Employer
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  May 2019
                  .item-description
                    p
                      | I was extremely impressed with the quality of work AND how quickly he got it done. He then offered to help with another side part of the project that we didn't even think about originally.
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | PHP Core Website Fixes 
                    span Rated as Freelancer
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  May 2019
                  .item-description
                    p
                      | Awesome work, definitely will rehire. Poject was completed not only with the requirements, but on time, within our small budget.
          // Pagination
          .clearfix
          .pagination-container.margin-top-40.margin-bottom-10
            nav.pagination
              ul
                li
                  a.ripple-effect.current-page(href='#') 1
                li
                  a.ripple-effect(href='#') 2
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-right
          .clearfix
          // Pagination / End
          // Boxed List / End
          // Boxed List
          .boxed-list.margin-bottom-60
            .boxed-list-headline
              h3
                i.icon-material-outline-business
                |  Employment History
            ul.boxed-list-ul
              li
                .boxed-list-item
                  // Avatar
                  .item-image
                    img(src='/images/browse-companies-03.png', alt='')
                  // Content
                  .item-content
                    h4 Development Team Leader
                    .item-details.margin-top-7
                      .detail-item
                        a(href='#')
                          i.icon-material-outline-business
                          |  Acodia
                      .detail-item
                        i.icon-material-outline-date-range
                        |  May 2019 - Present
                    .item-description
                      p
                        | Focus the team on the tasks at hand or the internal and external customer requirements.
              li
                .boxed-list-item
                  // Avatar
                  .item-image
                    img(src='/images/browse-companies-04.png', alt='')
                  // Content
                  .item-content
                    h4
                      a(href='#') Lead UX/UI Designer
                    .item-details.margin-top-7
                      .detail-item
                        a(href='#')
                          i.icon-material-outline-business
                          |  Acorta
                      .detail-item
                        i.icon-material-outline-date-range
                        |  April 2014 - May 2019
                    .item-description
                      p
                        | I designed and implemented 10+ custom web-based CRMs, workflow systems, payment solutions and mobile apps.
          // Boxed List / End
      // Sidebar
      .col-xl-4.col-lg-4
            .sidebar-container
              // Profile Overview
              .profile-overview
                .overview-item
                  strong $35
                  span Hourly Rate
                .overview-item
                  strong 53
                  span Jobs Done
                .overview-item
                  strong 22
                  span Rehired
              // Button
              a.apply-now-button.popup-with-zoom-anim.margin-bottom-50(href='#small-dialog')
                | Make an Offer 
                i.icon-material-outline-arrow-right-alt
              // Freelancer Indicators
              .sidebar-widget
                .freelancer-indicators
                  // Indicator
                  .indicator
                    strong 88%
                    .indicator-bar(data-indicator-percentage='88')
                      span
                    span Job Success
                  // Indicator
                  .indicator
                    strong 100%
                    .indicator-bar(data-indicator-percentage='100')
                      span
                    span Recommendation
                  // Indicator
                  .indicator
                    strong 90%
                    .indicator-bar(data-indicator-percentage='90')
                      span
                    span On Time
                  // Indicator
                  .indicator
                    strong 80%
                    .indicator-bar(data-indicator-percentage='80')
                      span
                    span On Budget
              // Widget
              .sidebar-widget
                h3 Social Profiles
                .freelancer-socials.margin-top-25
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
              // Widget
              .sidebar-widget
                h3 Skills
                .task-tags
                  span iOS
                  span Android
                  span mobile apps
                  span design
                  span Python
                  span Flask
                  span PHP
                  span WordPress
              // Widget
              .sidebar-widget
                h3 Attachments
                .attachments-container
                  a.attachment-box.ripple-effect(href='#')
                    span Cover Letter
                    i PDF
                  a.attachment-box.ripple-effect(href='#')
                    span Contract
                    i DOCX
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
  // Spacer
  .margin-top-15
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