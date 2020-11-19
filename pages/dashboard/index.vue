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
              li.active
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
        h3 Howdy, Tom!
        span We are glad to see you again!
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li Dashboard
      // Fun Facts Container
      .fun-facts-container
        .fun-fact(data-fun-fact-color='#36bd78')
          .fun-fact-text
            span Task Bids Won
            h4 22
          .fun-fact-icon
            i.icon-material-outline-gavel
        .fun-fact(data-fun-fact-color='#b81b7f')
          .fun-fact-text
            span Jobs Applied
            h4 4
          .fun-fact-icon
            i.icon-material-outline-business-center
        .fun-fact(data-fun-fact-color='#efa80f')
          .fun-fact-text
            span Reviews
            h4 28
          .fun-fact-icon
            i.icon-material-outline-rate-review
        // Last one has to be hidden below 1600px, sorry :(
        .fun-fact(data-fun-fact-color='#2a41e6')
          .fun-fact-text
            span This Month Views
            h4 987
          .fun-fact-icon
            i.icon-feather-trending-up
      // Row
      .row
        .col-xl-8
          // Dashboard Box
          .dashboard-box.main-box-in-row
            .headline
              h3
                i.icon-feather-bar-chart-2
                |  Your Profile Views
              .sort-by
                select.selectpicker.hide-tick
                  option Last 6 Months
                  option This Year
                  option This Month
            .content
              // Chart
              .chart
                canvas#chart(width='100', height='45')
          // Dashboard Box / End
        .col-xl-4
          // Dashboard Box
          //
            If you want adjust height of two boxes
            add to the lower box 'main-box-in-row'
            and 'child-box-in-row' to the higher box
          .dashboard-box.child-box-in-row
            .headline
              h3
                i.icon-material-outline-note-add
                |  Notes
            .content.with-padding
              // Note
              .dashboard-note
                p Meeting with candidate at 3pm who applied for Bilingual Event Support Specialist
                .note-footer
                  span.note-priority.high High Priority
                  .note-buttons
                    a(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a(href='#', title='Remove', data-tippy-placement='top')
                      i.icon-feather-trash-2
              // Note
              .dashboard-note
                p Extend premium plan for next month
                .note-footer
                  span.note-priority.low Low Priority
                  .note-buttons
                    a(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a(href='#', title='Remove', data-tippy-placement='top')
                      i.icon-feather-trash-2
              // Note
              .dashboard-note
                p Send payment to David Peterson
                .note-footer
                  span.note-priority.medium Medium Priority
                  .note-buttons
                    a(href='#', title='Edit', data-tippy-placement='top')
                      i.icon-feather-edit
                    a(href='#', title='Remove', data-tippy-placement='top')
                      i.icon-feather-trash-2
            .add-note-button
              a.popup-with-zoom-anim.button.full-width.button-sliding-icon(href='#small-dialog')
                | Add Note 
                i.icon-material-outline-arrow-right-alt
          // Dashboard Box / End
      // Row / End
      // Row
      .row
        // Dashboard Box
        .col-xl-6
          .dashboard-box
            .headline
              h3
                i.icon-material-baseline-notifications-none
                |  Notifications
              button.mark-as-read.ripple-effect-dark(data-tippy-placement='left', title='Mark all as read')
                i.icon-feather-check-square
            .content
              ul.dashboard-box-list
                li
                  span.notification-icon
                    i.icon-material-outline-group
                  span.notification-text
                    strong Michael Shannah
                    |  applied for a job 
                    a(href='#') Full Stack Software Engineer
                  // Buttons
                  .buttons-to-right
                    a.button.ripple-effect.ico(href='#', title='Mark as read', data-tippy-placement='left')
                      i.icon-feather-check-square
                li
                  span.notification-icon
                    i.icon-material-outline-gavel
                  span.notification-text
                    strong Gilber Allanis
                    |  placed a bid on your 
                    a(href='#') iOS App Development
                    |  project
                  // Buttons
                  .buttons-to-right
                    a.button.ripple-effect.ico(href='#', title='Mark as read', data-tippy-placement='left')
                      i.icon-feather-check-square
                li
                  span.notification-icon
                    i.icon-material-outline-autorenew
                  span.notification-text
                    | Your job listing 
                    a(href='#') Full Stack Software Engineer
                    |  is expiring
                  // Buttons
                  .buttons-to-right
                    a.button.ripple-effect.ico(href='#', title='Mark as read', data-tippy-placement='left')
                      i.icon-feather-check-square
                li
                  span.notification-icon
                    i.icon-material-outline-group
                  span.notification-text
                    strong Sindy Forrest
                    |  applied for a job 
                    a(href='#') Full Stack Software Engineer
                  // Buttons
                  .buttons-to-right
                    a.button.ripple-effect.ico(href='#', title='Mark as read', data-tippy-placement='left')
                      i.icon-feather-check-square
                li
                  span.notification-icon
                    i.icon-material-outline-rate-review
                  span.notification-text
                    strong David Peterson
                    |  left you a 
                    span.star-rating.no-stars(data-rating='5.0')
                    |  rating after finishing 
                    a(href='#') Logo Design
                    |  task
                  // Buttons
                  .buttons-to-right
                    a.button.ripple-effect.ico(href='#', title='Mark as read', data-tippy-placement='left')
                      i.icon-feather-check-square
        // Dashboard Box
        .col-xl-6
          .dashboard-box
            .headline
              h3
                i.icon-material-outline-assignment
                |  Orders
            .content
              ul.dashboard-box-list
                li
                  .invoice-list-item
                    strong Professional Plan
                    ul
                      li
                        span.unpaid Unpaid
                      li Order: #326
                      li Date: 12/08/2019
                  // Buttons
                  .buttons-to-right
                    a.button(href='pages-checkout-page.html') Finish Payment
                li
                  .invoice-list-item
                    strong Professional Plan
                    ul
                      li
                        span.paid Paid
                      li Order: #264
                      li Date: 10/07/2019
                  // Buttons
                  .buttons-to-right
                    a.button.gray(href='pages-invoice-template.html') View Invoice
                li
                  .invoice-list-item
                    strong Professional Plan
                    ul
                      li
                        span.paid Paid
                      li Order: #211
                      li Date: 12/06/2019
                  // Buttons
                  .buttons-to-right
                    a.button.gray(href='pages-invoice-template.html') View Invoice
                li
                  .invoice-list-item
                    strong Professional Plan
                    ul
                      li
                        span.paid Paid
                      li Order: #179
                      li Date: 06/05/2019
                  // Buttons
                  .buttons-to-right
                    a.button.gray(href='pages-invoice-template.html') View Invoice
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