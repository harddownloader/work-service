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
              li.active-submenu
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
        h3 Manage Bidders
        span.margin-top-7
          | Bids for 
          a(href='#') Food Delivery Mobile Application
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Manage Bidders
      // Row
      .row
        // Dashboard Box
        .col-xl-12
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-material-outline-supervisor-account
                |  3 Bidders
              .sort-by
                select.selectpicker.hide-tick
                  option Highest First
                  option Lowest First
                  option Fastest First
            .content
              ul.dashboard-box-list
                li
                  // Overview
                  .freelancer-overview.manage-candidates
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
                        // Details
                        span.freelancer-detail-item
                          a(href='#')
                            i.icon-feather-mail
                            |  david@example.com
                        // Rating
                        .freelancer-rating
                          .star-rating(data-rating='5.0')
                        // Bid Details
                        ul.dashboard-task-info.bid-info
                          li
                            strong $3,200
                            span Fixed Price
                          li
                            strong 14 Days
                            span Delivery Time
                        // Buttons
                        .buttons-to-right.always-visible.margin-top-25.margin-bottom-0
                          a.popup-with-zoom-anim.button.ripple-effect(href='#small-dialog-1')
                            i.icon-material-outline-check
                            |  Accept Offer
                          a.popup-with-zoom-anim.button.dark.ripple-effect(href='#small-dialog-2')
                            i.icon-feather-mail
                            |  Send Message
                          a.button.gray.ripple-effect.ico(href='#', title='Remove Bid', data-tippy-placement='top')
                            i.icon-feather-trash-2
                li
                  // Overview
                  .freelancer-overview.manage-candidates
                    .freelancer-overview-inner
                      // Avatar
                      .freelancer-avatar
                        a(href='#')
                          img(src='images/user-avatar-placeholder.png', alt='')
                      // Name
                      .freelancer-name
                        h4
                          a(href='#')
                            | Oldrich Ćuk 
                            img.flag(src='images/flags/sk.svg', alt='', title='Slovakia', data-tippy-placement='top')
                        // Details
                        span.freelancer-detail-item
                          a(href='#')
                            i.icon-feather-mail
                            |  oldrich@example.com
                        span.freelancer-detail-item
                          i.icon-feather-phone
                          |  (+421) 123-456-789
                        // Rating
                        br
                        span.company-not-rated Minimum of 3 votes required
                        // Bid Details
                        ul.dashboard-task-info.bid-info
                          li
                            strong $3,000
                            span Fixed Price
                          li
                            strong 14 Days
                            span Delivery Time
                        // Buttons
                        .buttons-to-right.always-visible.margin-top-25.margin-bottom-0
                          a.popup-with-zoom-anim.button.ripple-effect(href='#small-dialog-1')
                            i.icon-material-outline-check
                            |  Accept Offer
                          a.popup-with-zoom-anim.button.dark.ripple-effect(href='#small-dialog-2')
                            i.icon-feather-mail
                            |  Send Message
                          a.button.gray.ripple-effect.ico(href='#', title='Remove Bid', data-tippy-placement='top')
                            i.icon-feather-trash-2
                li
                  // Overview
                  .freelancer-overview.manage-candidates
                    .freelancer-overview-inner
                      // Avatar
                      .freelancer-avatar
                        .verified-badge
                        a(href='#')
                          img(src='images/user-avatar-placeholder.png', alt='')
                      // Name
                      .freelancer-name
                        h4
                          a(href='#')
                            | Kuba Adamczyk 
                            img.flag(src='images/flags/pl.svg', alt='', title='Poland', data-tippy-placement='top')
                        // Details
                        span.freelancer-detail-item
                          a(href='#')
                            i.icon-feather-mail
                            |  kuba@example.com
                        span.freelancer-detail-item
                          i.icon-feather-phone
                          |  (+48) 123-456-789
                        // Rating
                        .freelancer-rating
                          .star-rating(data-rating='5.0')
                        // Bid Details
                        ul.dashboard-task-info.bid-info
                          li
                            strong $2,700
                            span Fixed Price
                          li
                            strong 30 Days
                            span Delivery Time
                        // Buttons
                        .buttons-to-right.always-visible.margin-top-25.margin-bottom-0
                          a.popup-with-zoom-anim.button.ripple-effect(href='#small-dialog-1')
                            i.icon-material-outline-check
                            |  Accept Offer
                          a.popup-with-zoom-anim.button.dark.ripple-effect(href='#small-dialog-2')
                            i.icon-feather-mail
                            |  Send Message
                          a.button.gray.ripple-effect.ico(href='#', title='Remove Bid', data-tippy-placement='top')
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