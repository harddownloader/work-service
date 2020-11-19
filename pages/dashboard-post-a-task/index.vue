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
        h3 Post a Task
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Post a Task
      // Row
      .row
        // Dashboard Box
        .col-xl-12
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-feather-folder-plus
                |  Task Submission Form
            .content.with-padding.padding-bottom-10
              .row
                .col-xl-4
                  .submit-field
                    h5 Project Name
                    input.with-border(type='text', placeholder='e.g. build me a website')
                .col-xl-4
                  .submit-field
                    h5 Category
                    select.selectpicker.with-border(data-size='7', title='Select Category')
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
                .col-xl-4
                  .submit-field
                    h5
                      | Location  
                      i.help-icon(data-tippy-placement='right', title="Leave blank if it's an online job")
                    .input-with-icon
                      #autocomplete-container
                        input#autocomplete-input.with-border(type='text', placeholder='Anywhere')
                      i.icon-material-outline-location-on
                .col-xl-6
                  .submit-field
                    h5 What is your estimated budget?
                    .row
                      .col-xl-6
                        .input-with-icon
                          input.with-border(type='text', placeholder='Minimum')
                          i.currency USD
                      .col-xl-6
                        .input-with-icon
                          input.with-border(type='text', placeholder='Maximum')
                          i.currency USD
                    .feedback-yes-no.margin-top-0
                      .radio
                        input#radio-1(name='radio', type='radio', checked='')
                        label(for='radio-1')
                          span.radio-label
                          |  Fixed Price Project
                      .radio
                        input#radio-2(name='radio', type='radio')
                        label(for='radio-2')
                          span.radio-label
                          |  Hourly Project
                .col-xl-6
                  .submit-field
                    h5
                      | What skills are required? 
                      i.help-icon(data-tippy-placement='right', title='Up to 5 skills that best describe your project')
                    .keywords-container
                      .keyword-input-container
                        input.keyword-input.with-border(type='text', placeholder='Add Skills')
                        button.keyword-input-button.ripple-effect
                          i.icon-material-outline-add
                      .keywords-list
                        // keywords go here
                      .clearfix
                .col-xl-12
                  .submit-field
                    h5 Describe Your Project
                    textarea.with-border(cols='30', rows='5')
                    .uploadButton.margin-top-30
                      input#upload.uploadButton-input(type='file', accept='image/*, application/pdf', multiple='')
                      label.uploadButton-button.ripple-effect(for='upload') Upload Files
                      span.uploadButton-file-name Images or documents that might be helpful in describing your project
        .col-xl-12
          a.button.ripple-effect.big.margin-top-30(href='#')
            i.icon-feather-plus
            |  Post a Task
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