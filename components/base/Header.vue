<template lang="pug">

  //
    Header Container //.fullwidth
    ==================================================
  header#header-container(v-bind:class="headerClassObj") 
    // Header
    #header
      .container
        // Left Side Content
        .left-side
          // Logo
          #logo
            nuxt-link.current(to='/')
              img(src='/images/logo.png', alt='')
          // Main Navigation
          nav#navigation
            ul#responsive
              li
                nuxt-link.current(to='/') Home
                //- ul.dropdown-nav
                  li
                    a(href='index.html') Home 1
                  li
                    a(href='index-2.html') Home 2
                  li
                    a(href='index-3.html') Home 3
              li
                a(href='#') Find Work
                ul.dropdown-nav
                  li
                    //- a(href='#') Browse Jobs
                    nuxt-link(to="/browse-jobs") Browse Jobs
                    //- ul.dropdown-nav
                      li
                        a(href='jobs-list-layout-full-page-map.html') Full Page List + Map
                      li
                        a(href='jobs-grid-layout-full-page-map.html') Full Page Grid + Map
                      li
                        a(href='jobs-grid-layout-full-page.html') Full Page Grid
                      li
                        a(href='jobs-list-layout-1.html') List Layout 1
                      li
                        a(href='jobs-list-layout-2.html') List Layout 2
                      li
                        a(href='jobs-grid-layout.html') Grid Layout
                  li
                    nuxt-link(to="/browse-tasks") Browse Tasks
                    //- a(href='#') Browse Tasks
                    //- ul.dropdown-nav
                      li
                        a(href='tasks-list-layout-1.html') List Layout 1
                      li
                        a(href='tasks-list-layout-2.html') List Layout 2
                      li
                        a(href='tasks-grid-layout.html') Grid Layout
                      li
                        a(href='tasks-grid-layout-full-page.html') Full Page Grid
                  li
                    //- a(href='browse-companies.html') Browse Companies
                    nuxt-link(to="/browse-companies") Browse Companies
                  li
                    //- a(href='single-job-page.html') Job Page
                    nuxt-link(to="/single-job-page") Job Page
                  li
                    //- a(href='single-task-page.html') Task Page
                    nuxt-link(to="/single-task-page") Task Page
                  li
                    //- a(href='single-company-profile.html') Company Profile
                    nuxt-link(to="/single-company-profile") Company Profile
              li
                //- a(href='#') For Employers
                nuxt-link(to="freelancers-list") For Employers
                ul.dropdown-nav
                  li
                    //- a(href='#') Find a Freelancer
                    nuxt-link(to="freelancers-list") Find a Freelancer
                    //- ul.dropdown-nav
                      li
                        a(href='freelancers-grid-layout-full-page.html') Full Page Grid
                      li
                        a(href='freelancers-grid-layout.html') Grid Layout
                      li
                        a(href='freelancers-list-layout-1.html') List Layout 1
                      li
                        a(href='freelancers-list-layout-2.html') List Layout 2
                  li
                    //- a(href='single-freelancer-profile.html') Freelancer Profile
                    nuxt-link(to="single-freelancer-profile") Freelancer Profile
                  li
                    //- a(href='dashboard-post-a-job.html') Post a Job
                    nuxt-link(to="dashboard-post-a-job") Post a Job
                  li
                    //- a(href='dashboard-post-a-task.html') Post a Task
                    nuxt-link(to="dashboard-post-a-task") Post a Task
              li
                a(href='#') Dashboard
                ul.dropdown-nav
                  li
                    //- a(href='dashboard.html') Dashboard
                    nuxt-link(to="dashboard") Dashboard
                  li
                    //- a(href='dashboard-messages.html') Messages
                    nuxt-link(to="dashboard-messages") Messages
                  li
                    //- a(href='dashboard-bookmarks.html') Bookmarks
                    nuxt-link(to="dashboard-bookmarks") Bookmarks
                  li
                    //- a(href='dashboard-reviews.html') Reviews
                    nuxt-link(to="dashboard-reviews") Reviews
                  li
                    //- a(href='dashboard-manage-jobs.html') Jobs
                    nuxt-link(to="dashboard-manage-jobs") Jobs
                    ul.dropdown-nav
                      li
                        //- a(href='dashboard-manage-jobs.html') Manage Jobs
                        nuxt-link(to="dashboard-manage-jobs") Manage Jobs
                      li
                        //- a(href='dashboard-manage-candidates.html') Manage Candidates
                        nuxt-link(to="dashboard-manage-candidates") Manage Candidates
                      li
                        //- a(href='dashboard-post-a-job.html') Post a Job
                        nuxt-link(to="dashboard-post-a-job") Post a Job
                  li
                    //- a(href='dashboard-manage-tasks.html') Tasks
                    nuxt-link(to="dashboard-manage-tasks") Tasks
                    ul.dropdown-nav
                      li
                        //- a(href='dashboard-manage-tasks.html') Manage Tasks
                        nuxt-link(to="dashboard-manage-tasks") Manage Tasks
                      li
                        //- a(href='dashboard-manage-bidders.html') Manage Bidders
                        nuxt-link(to="dashboard-manage-bidders") Manage Bidders
                      li
                        //- a(href='dashboard-my-active-bids.html') My Active Bids
                        nuxt-link(to="dashboard-my-active-bids") My Active Bids
                      li
                        //- a(href='dashboard-post-a-task.html') Post a Task
                        nuxt-link(to="dashboard-post-a-task") Post a Task
                  li
                    //- a(href='dashboard-settings.html') Settings
                    nuxt-link(to="dashboard-settings") Settings
              li
                a(href='#') Pages
                ul.dropdown-nav
                  li
                    a(href='#') Open Street Map
                    ul.dropdown-nav
                      li
                        a(href='jobs-list-layout-full-page-map-OpenStreetMap.html') Full Page List + Map
                      li
                        a(href='jobs-grid-layout-full-page-map-OpenStreetMap.html') Full Page Grid + Map
                      li
                        a(href='single-job-page-OpenStreetMap.html') Job Page
                      li
                        a(href='single-company-profile-OpenStreetMap.html') Company Profile
                      li
                        a(href='pages-contact-OpenStreetMap.html') Contact
                      li
                        a(href='jobs-list-layout-1-OpenStreetMap.html') Location Autocomplete
                  li
                    //- a(href='pages-blog.html') Blog
                    nuxt-link(to="pages-blog") Blog
                  li
                    a(href='pages-pricing-plans.html') Pricing Plans
                  li
                    //- a(href='pages-checkout-page.html') Checkout Page
                    nuxt-link(to="pages-checkout-page") Checkout Page
                  li
                    //- a(href='pages-invoice-template.html') Invoice Template
                    nuxt-link(to="pages-invoice-template") Invoice Template
                  li
                    a(href='pages-user-interface-elements.html') User Interface Elements
                  li
                    a(href='pages-icons-cheatsheet.html') Icons Cheatsheet
                  li
                    //- a(href='pages-login.html') Login & Register
                    nuxt-link(to="pages-login") Login & Register
                  li
                    a(href='pages-404.html') 404 Page
                  li
                    //- a(href='pages-contact.html') Contact
                    nuxt-link(to="pages-contact") Contact
          .clearfix
          // Main Navigation / End
          // Left Side Content / End
        // Right Side Content / End
        .right-side
          // User Notifications
          .header-widget.hide-on-mobile
            // Notifications
            .header-notifications
              // Trigger
              .header-notifications-trigger
                a(href='#')
                  i.icon-feather-bell
                  span 4
              // Dropdown
              .header-notifications-dropdown
                .header-notifications-headline
                  h4 Notifications
                  button.mark-as-read.ripple-effect-dark(title='Mark all as read', data-tippy-placement='left')
                    i.icon-feather-check-square
                .header-notifications-content
                  .header-notifications-scroll(data-simplebar='')
                    ul
                      // Notification
                      li.notifications-not-read
                        a(href='dashboard-manage-candidates.html')
                          span.notification-icon
                            i.icon-material-outline-group
                          span.notification-text
                            strong Michael Shannah
                            |  applied for a job 
                            span.color Full Stack Software Engineer
                      // Notification
                      li
                        a(href='dashboard-manage-bidders.html')
                          span.notification-icon
                            i.icon-material-outline-gavel
                          span.notification-text
                            strong Gilbert Allanis
                            |  placed a bid on your 
                            span.color iOS App Development
                            |  project
                      // Notification
                      li
                        a(href='dashboard-manage-jobs.html')
                          span.notification-icon
                            i.icon-material-outline-autorenew
                          span.notification-text
                            | Your job listing 
                            span.color Full Stack PHP Developer
                            |  is expiring.
                      // Notification
                      li
                        a(href='dashboard-manage-candidates.html')
                          span.notification-icon
                            i.icon-material-outline-group
                          span.notification-text
                            strong Sindy Forrest
                            |  applied for a job 
                            span.color Full Stack Software Engineer
            // Messages
            .header-notifications
              .header-notifications-trigger
                a(href='#')
                  i.icon-feather-mail
                  span 3
              // Dropdown
              .header-notifications-dropdown
                .header-notifications-headline
                  h4 Messages
                  button.mark-as-read.ripple-effect-dark(title='Mark all as read', data-tippy-placement='left')
                    i.icon-feather-check-square
                .header-notifications-content
                  .header-notifications-scroll(data-simplebar='')
                    ul
                      // Notification
                      li.notifications-not-read
                        a(href='dashboard-messages.html')
                          span.notification-avatar.status-online
                            img(src='~static/images/user-avatar-small-03.jpg', alt='')
                          .notification-text
                            strong David Peterson
                            p.notification-msg-text Thanks for reaching out. I'm quite busy right now on many...
                            span.color 4 hours ago
                      // Notification
                      li.notifications-not-read
                        a(href='dashboard-messages.html')
                          span.notification-avatar.status-offline
                            img(src='/images/user-avatar-small-02.jpg', alt='')
                          .notification-text
                            strong Sindy Forest
                            p.notification-msg-text Hi Tom! Hate to break it to you, but I'm actually on vacation until...
                            span.color Yesterday
                      // Notification
                      li.notifications-not-read
                        a(href='dashboard-messages.html')
                          span.notification-avatar.status-online
                            img(src='/images/user-avatar-placeholder.png', alt='')
                          .notification-text
                            strong Marcin Kowalski
                            p.notification-msg-text I received payment. Thanks for cooperation!
                            span.color Yesterday
                a.header-notifications-button.ripple-effect.button-sliding-icon(href='dashboard-messages.html')
                  | View All Messages
                  i.icon-material-outline-arrow-right-alt
          // User Notifications / End
          // User Menu
          .header-widget
            // Messages
            .header-notifications.user-menu
              .header-notifications-trigger
                a(href='#')
                  .user-avatar.status-online
                    img(src='/images/user-avatar-small-01.jpg', alt='')
              // Dropdown
              .header-notifications-dropdown
                // User Status
                .user-status
                  // User Name / Avatar
                  .user-details
                    .user-avatar.status-online
                      img(src='/images/user-avatar-small-01.jpg', alt='')
                    .user-name
                      | Tom Smith 
                      span Freelancer
                  // User Status Switcher
                  #snackbar-user-status.status-switch
                    label.user-online.current-status Online
                    label.user-invisible Invisible
                    // Status Indicator
                    span.status-indicator(aria-hidden='true')
                ul.user-menu-small-nav
                  li
                    a(href='dashboard.html')
                      i.icon-material-outline-dashboard
                      |  Dashboard
                  li
                    a(href='dashboard-settings.html')
                      i.icon-material-outline-settings
                      |  Settings
                  li
                    a(href='index-logged-out.html')
                      i.icon-material-outline-power-settings-new
                      |  Logout
          // User Menu / End
          // Mobile Navigation Button
          span.mmenu-trigger
            button.hamburger.hamburger--collapse(type='button')
              span.hamburger-box
                span.hamburger-inner
        // Right Side Content / End
        // Header / End
  

</template>

<script>
  export default {
    props: ['layout'],
    data: () => {
      return {
        
      }
    },
    computed: {
      headerClassObj: function () {
        return {
            'fullwidth': true,
            'dashboard-header not-sticky': this.layout === 'dashboard'
          }
      }
    } 
  }
</script>

<style lang="stylus" scoped>

</style>