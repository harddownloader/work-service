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
              li.active
                a(href='dashboard-bookmarks.html')
                  i.icon-material-outline-star-border
                  |  Bookmarks
              li
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
        h3 Bookmarks
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Bookmarks
      // Row
      .row
        // Dashboard Box
        .col-xl-12
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-material-outline-business-center
                |  Bookmarked Jobs
            .content
              ul.dashboard-box-list
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Logo
                      a.job-listing-company-logo(href='#')
                        img(src='images/company-logo-02.png', alt='')
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Barista and Cashier
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-business
                              |  Coffee
                            li
                              i.icon-material-outline-location-on
                              |  San Francisco
                            li
                              i.icon-material-outline-business-center
                              |  Full Time
                            li
                              i.icon-material-outline-access-time
                              |  2 days ago
                  // Buttons
                  .buttons-to-right
                    a.button.red.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='left')
                      i.icon-feather-trash-2
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Logo
                      a.job-listing-company-logo(href='#')
                        img(src='images/company-logo-04.png', alt='')
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Administrative Assistant
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-business
                              |  Mates
                            li
                              i.icon-material-outline-location-on
                              |  San Francisco
                            li
                              i.icon-material-outline-business-center
                              |  Full Time
                            li
                              i.icon-material-outline-access-time
                              |  2 days ago
                  // Buttons
                  .buttons-to-right
                    a.button.red.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='left')
                      i.icon-feather-trash-2
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Logo
                      a.job-listing-company-logo(href='#')
                        img(src='images/company-logo-05.png', alt='')
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Construction Labourers
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-business
                              |  Podous
                            li
                              i.icon-material-outline-location-on
                              |  San Francisco
                            li
                              i.icon-material-outline-business-center
                              |  Full Time
                            li
                              i.icon-material-outline-access-time
                              |  2 days ago
                  // Buttons
                  .buttons-to-right
                    a.button.red.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='left')
                      i.icon-feather-trash-2
        // Dashboard Box
        .col-xl-12
          .dashboard-box
            // Headline
            .headline
              h3
                i.icon-material-outline-face
                |  Bookmarked Freelancers
            .content
              ul.dashboard-box-list
                li
                  // Overview
                  .freelancer-overview
                    .freelancer-overview-inner
                      // Avatar
                      .freelancer-avatar
                        .verified-badge
                        a(href='#')
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
                  // Buttons
                  .buttons-to-right
                    a.button.red.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='left')
                      i.icon-feather-trash-2
                li
                  // Overview
                  .freelancer-overview
                    .freelancer-overview-inner
                      // Avatar
                      .freelancer-avatar
                        a(href='#')
                          img(src='images/user-avatar-placeholder.png', alt='')
                      // Name
                      .freelancer-name
                        h4
                          a(href='#')
                            | Marcin Kowalski 
                            img.flag(src='images/flags/pl.svg', alt='', title='Poland', data-tippy-placement='top')
                        span Front-End Developer
                        // Rating
                        .freelancer-rating
                          .star-rating(data-rating='4.7')
                  // Buttons
                  .buttons-to-right
                    a.button.red.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='left')
                      i.icon-feather-trash-2
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