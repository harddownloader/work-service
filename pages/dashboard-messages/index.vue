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
              li.active
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
        h3 Messages
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Messages
      .messages-container.margin-top-0
        .messages-container-inner
          // Messages
          .messages-inbox
            .messages-headline
              .input-with-icon
                input#autocomplete-input(type='text', placeholder='Search')
                i.icon-material-outline-search
            ul
              li
                a(href='#')
                  .message-avatar
                    i.status-icon.status-online
                    img(src='images/user-avatar-small-03.jpg', alt='')
                  .message-by
                    .message-by-headline
                      h5 David Peterson
                      span 4 hours ago
                    p Thanks for reaching out. I'm quite busy right now on many
              li.active-message
                a(href='#')
                  .message-avatar
                    i.status-icon.status-offline
                    img(src='images/user-avatar-small-02.jpg', alt='')
                  .message-by
                    .message-by-headline
                      h5 Sindy Forest
                      span Yesterday
                    p Hi Tom! Hate to break it to you but I'm actually on vacation
              li
                a(href='#')
                  .message-avatar
                    i.status-icon.status-offline
                    img(src='images/user-avatar-placeholder.png', alt='')
                  .message-by
                    .message-by-headline
                      h5 Sebastiano Piccio
                      span 2 days ago
                    p Hello, I want to talk about my project if you don't mind!
              li
                a(href='#')
                  .message-avatar
                    i.status-icon.status-online
                    img(src='images/user-avatar-placeholder.png', alt='')
                  .message-by
                    .message-by-headline
                      h5 Marcin Kowalski
                      span 2 days ago
                    p Yes, I received payment. Thanks for cooperation!
          // Messages / End
          // Message Content
          .message-content
            .messages-headline
              h4 Sindy Forest
              a.message-action(href='#')
                i.icon-feather-trash-2
                |  Delete Conversation
            // Message Content Inner
            .message-content-inner
              // Time Sign
              .message-time-sign
                span 28 June, 2019
              .message-bubble.me
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-01.jpg', alt='')
                  .message-text
                    p Thanks for choosing my offer. I will start working on your project tomorrow.
                .clearfix
              .message-bubble
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-02.jpg', alt='')
                  .message-text
                    p Great. If you need any further clarification let me know. 👍
                .clearfix
              .message-bubble.me
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-01.jpg', alt='')
                  .message-text
                    p Ok, I will. 😉
                .clearfix
              // Time Sign
              .message-time-sign
                span Yesterday
              .message-bubble.me
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-01.jpg', alt='')
                  .message-text
                    p
                      | Hi Sindy, I just wanted to let you know that project is finished and I'm waiting for your approval.
                .clearfix
              .message-bubble
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-02.jpg', alt='')
                  .message-text
                    p
                      | Hi Tom! Hate to break it to you, but I'm actually on vacation 🌴 until Sunday so I can't check it now. 😎
                .clearfix
              .message-bubble.me
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-01.jpg', alt='')
                  .message-text
                    p Ok, no problem. But don't forget about last payment. 🙂
                .clearfix
              .message-bubble
                .message-bubble-inner
                  .message-avatar
                    img(src='images/user-avatar-small-02.jpg', alt='')
                  .message-text
                    // Typing Indicator
                    .typing-indicator
                      span
                      span
                      span
                .clearfix
            // Message Content Inner / End
            // Reply Area
            .message-reply
              textarea(cols='1', rows='1', placeholder='Your Message', data-autoresize='')
              button.button.ripple-effect Send
          // Message Content
      // Messages Container / End
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