<template lang="pug">
// Dashboard Container
.dashboard-container
  //
    Dashboard Sidebar
    ==================================================
  .dashboard-sidebar
    .dashboard-sidebar-inner(data-simplebar='')
      .dashboard-nav-container
        // Responsive Navigation Trigger
        a.dashboard-responsive-nav-trigger(href='#')
          span.hamburger.hamburger--collapse
            span.hamburger-box
              span.hamburger-inner
          span.trigger-title Dashboard Navigation
        // Navigation
        .dashboard-nav
          .dashboard-nav-inner
            ul(data-submenu-title='Start')
              li
                a(href='dashboard.html')
                  i.icon-material-outline-dashboard
                  |  Dashboard
              li
                a(href='dashboard-messages.html')
                  i.icon-material-outline-question-answer
                  |  Messages 
                  span.nav-tag 2
              li
                a(href='dashboard-bookmarks.html')
                  i.icon-material-outline-star-border
                  |  Bookmarks
              li.active
                a(href='dashboard-reviews.html')
                  i.icon-material-outline-rate-review
                  |  Reviews
            ul(data-submenu-title='Organize and Manage')
              li
                a(href='#')
                  i.icon-material-outline-business-center
                  |  Jobs
                ul
                  li
                    a(href='dashboard-manage-jobs.html')
                      | Manage Jobs 
                      span.nav-tag 3
                  li
                    a(href='dashboard-manage-candidates.html') Manage Candidates
                  li
                    a(href='dashboard-post-a-job.html') Post a Job
              li
                a(href='#')
                  i.icon-material-outline-assignment
                  |  Tasks
                ul
                  li
                    a(href='dashboard-manage-tasks.html')
                      | Manage Tasks 
                      span.nav-tag 2
                  li
                    a(href='dashboard-manage-bidders.html') Manage Bidders
                  li
                    a(href='dashboard-my-active-bids.html')
                      | My Active Bids 
                      span.nav-tag 4
                  li
                    a(href='dashboard-post-a-task.html') Post a Task
            ul(data-submenu-title='Account')
              li
                a(href='dashboard-settings.html')
                  i.icon-material-outline-settings
                  |  Settings
              li
                a(href='index-logged-out.html')
                  i.icon-material-outline-power-settings-new
                  |  Logout
        // Navigation / End
  // Dashboard Sidebar / End
  //
    Dashboard Content
    ==================================================
  .dashboard-content-container(data-simplebar='')
    .dashboard-content-inner
      // Dashboard Headline
      .dashboard-headline
        h3 Reviews
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Reviews
      // Row
      .row
        // Dashboard Box
        .col-xl-6
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-material-outline-business
                |  Rate Employers
            .content
              ul.dashboard-box-list
                li
                  .boxed-list-item
                    // Content
                    .item-content
                      h4 Simple Chrome Extension
                      span.company-not-rated.margin-bottom-5 Not Rated
                  a.popup-with-zoom-anim.button.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-2')
                    i.icon-material-outline-thumb-up
                    |  Leave a Review
                li
                  .boxed-list-item
                    // Content
                    .item-content
                      h4 Adsense Expert
                      span.company-not-rated.margin-bottom-5 Not Rated
                  a.popup-with-zoom-anim.button.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-2')
                    i.icon-material-outline-thumb-up
                    |  Leave a Review
                li
                  .boxed-list-item
                    // Content
                    .item-content
                      h4 Fix Python Selenium Code
                      .item-details.margin-top-10
                        .star-rating(data-rating='5.0')
                        .detail-item
                          i.icon-material-outline-date-range
                          |  May 2019
                      .item-description
                        p
                          | Great clarity in specification and communication. I got payment really fast. Really recommend this employer for his professionalism. I will work for him again with pleasure.
                  a.popup-with-zoom-anim.button.gray.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-1')
                    i.icon-feather-edit
                    |  Edit Review
                li
                  .boxed-list-item
                    // Content
                    .item-content
                      h4 PHP Core Website Fixes
                      .item-details.margin-top-10
                        .star-rating(data-rating='5.0')
                        .detail-item
                          i.icon-material-outline-date-range
                          |  May 2019
                      .item-description
                        p
                          | Great clarity in specification and communication. I got payment really fast. Really recommend this employer for his professionalism. I will work for him again with pleasure.
                  a.popup-with-zoom-anim.button.gray.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-1')
                    i.icon-feather-edit
                    |  Edit Review
          // Pagination
          .clearfix
          .pagination-container.margin-top-40.margin-bottom-0
            nav.pagination
              ul
                li
                  a.ripple-effect.current-page(href='#') 1
                li
                  a.ripple-effect(href='#') 2
                li
                  a.ripple-effect(href='#') 3
                li.pagination-arrow
                  a.ripple-effect(href='#')
                    i.icon-material-outline-keyboard-arrow-right
          .clearfix
          // Pagination / End
          // Dashboard Box
        .col-xl-6
            .dashboard-box.margin-top-0
              // Headline
              .headline
                h3
                  i.icon-material-outline-face
                  |  Rate Freelancers
              .content
                ul.dashboard-box-list
                  li
                    .boxed-list-item
                      // Content
                      .item-content
                        h4 Simple Chrome Extension
                        span.company-not-rated.margin-bottom-5 Not Rated
                    a.popup-with-zoom-anim.button.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-2')
                      i.icon-material-outline-thumb-up
                      |  Leave a Review
                  li
                    .boxed-list-item
                      // Content
                      .item-content
                        h4 Help Fix Laravel PHP issue
                        .item-details.margin-top-10
                          .star-rating(data-rating='5.0')
                          .detail-item
                            i.icon-material-outline-date-range
                            |  August 2019
                        .item-description
                          p Excellent programmer - helped me fixing small issue.
                    a.popup-with-zoom-anim.button.gray.ripple-effect.margin-top-5.margin-bottom-10(href='#small-dialog-1')
                      i.icon-feather-edit
                      |  Edit Review
      // Row / End
      // Footer
      .dashboard-footer-spacer
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
      // Dashboard Content / End
// Dashboard Container / End

</template>

<script>

  export default {
    layout: 'dashboard',
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