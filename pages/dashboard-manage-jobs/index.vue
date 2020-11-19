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
              li
                a(href='dashboard-reviews.html')
                  i.icon-material-outline-rate-review
                  |  Reviews
            ul(data-submenu-title='Organize and Manage')
              li.active-submenu
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
        h3 Manage Jobs
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Manage Jobs
      // Row
      .row
        // Dashboard Box
        .col-xl-12
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-material-outline-business-center
                |  My Job Listings
            .content
              ul.dashboard-box-list
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Logo
                      //
                        <a href="#" class="job-listing-company-logo">
                        <img src="images/company-logo-05.png" alt="">
                        </a>
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Frontend React Developer
                          span.dashboard-status-button.green Pending Approval
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-date-range
                              |  Posted on 10 July, 2019
                            li
                              i.icon-material-outline-date-range
                              |  Expiring on 10 August, 2019
                  // Buttons
                  .buttons-to-right.always-visible
                    a.button.ripple-effect(href='dashboard-manage-candidates.html')
                      i.icon-material-outline-supervisor-account
                      |  Manage Candidates 
                      span.button-info 0
                    a.button.gray.ripple-effect.ico(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a.button.gray.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='top')
                      i.icon-feather-trash-2
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Full Stack PHP Developer
                          span.dashboard-status-button.yellow Expiring
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-date-range
                              |  Posted on 28 June, 2019
                            li
                              i.icon-material-outline-date-range
                              |  Expiring on 28 July, 2019
                  // Buttons
                  .buttons-to-right.always-visible
                    a.button.ripple-effect(href='dashboard-manage-candidates.html')
                      i.icon-material-outline-supervisor-account
                      |  Manage Candidates 
                      span.button-info 3
                    a.button.gray.ripple-effect.ico(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a.button.gray.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='top')
                      i.icon-feather-trash-2
                li
                  // Job Listing
                  .job-listing
                    // Job Listing Details
                    .job-listing-details
                      // Details
                      .job-listing-description
                        h3.job-listing-title
                          a(href='#') Node.js Developer
                          span.dashboard-status-button.red Expired
                        // Job Listing Footer
                        .job-listing-footer
                          ul
                            li
                              i.icon-material-outline-date-range
                              |  Posted on 16 May, 2019
                  // Buttons
                  .buttons-to-right.always-visible
                    a.button.ripple-effect(href='dashboard-manage-candidates.html')
                      i.icon-material-outline-supervisor-account
                      |  Manage Candidates 
                      span.button-info 7
                    a.button.dark.ripple-effect(href='#')
                      i.icon-feather-rotate-ccw
                      |  Refresh
                    a.button.gray.ripple-effect.ico(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a.button.gray.ripple-effect.ico(href='#', title='Remove', data-tippy-placement='top')
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