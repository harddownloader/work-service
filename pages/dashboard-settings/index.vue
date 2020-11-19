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
              li.active
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
        h3 Settings
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            li
              a(href='#') Home
            li
              a(href='#') Dashboard
            li Settings
      // Row
      .row
        // Dashboard Box
        .col-xl-12
          .dashboard-box.margin-top-0
            // Headline
            .headline
              h3
                i.icon-material-outline-account-circle
                |  My Account
            .content.with-padding.padding-bottom-0
              .row
                .col-auto
                  .avatar-wrapper(data-tippy-placement='bottom', title='Change Avatar')
                    img.profile-pic(src='images/user-avatar-placeholder.png', alt='')
                    .upload-button
                    input.file-upload(type='file', accept='image/*')
                .col
                  .row
                    .col-xl-6
                      .submit-field
                        h5 First Name
                        input.with-border(type='text', value='Tom')
                    .col-xl-6
                      .submit-field
                        h5 Last Name
                        input.with-border(type='text', value='Smith')
                    .col-xl-6
                      // Account Type
                      .submit-field
                        h5 Account Type
                        .account-type
                          div
                            input#freelancer-radio.account-type-radio(type='radio', name='account-type-radio', checked='')
                            label.ripple-effect-dark(for='freelancer-radio')
                              i.icon-material-outline-account-circle
                              |  Freelancer
                          div
                            input#employer-radio.account-type-radio(type='radio', name='account-type-radio')
                            label.ripple-effect-dark(for='employer-radio')
                              i.icon-material-outline-business-center
                              |  Employer
                    .col-xl-6
                      .submit-field
                        h5 Email
                        input.with-border(type='text', value='tom@example.com')
        // Dashboard Box
        .col-xl-12
          .dashboard-box
            // Headline
            .headline
              h3
                i.icon-material-outline-face
                |  My Profile
            .content
              ul.fields-ul
                li
                  .row
                    .col-xl-4
                      .submit-field
                        .bidding-widget
                          // Headline
                          span.bidding-detail
                            | Set your 
                            strong minimal hourly rate
                          // Slider
                          .bidding-value.margin-bottom-10
                            | $
                            span#biddingVal
                          input.bidding-slider(type='text', value='', data-slider-handle='custom', data-slider-currency='$', data-slider-min='5', data-slider-max='150', data-slider-value='35', data-slider-step='1', data-slider-tooltip='hide')
                    .col-xl-4
                      .submit-field
                        h5
                          | Skills 
                          i.help-icon(data-tippy-placement='right', title='Add up to 10 skills')
                        // Skills List
                        .keywords-container
                          .keyword-input-container
                            input.keyword-input.with-border(type='text', placeholder='e.g. Angular, Laravel')
                            button.keyword-input-button.ripple-effect
                              i.icon-material-outline-add
                          .keywords-list
                            span.keyword
                              span.keyword-remove
                              span.keyword-text Angular
                            span.keyword
                              span.keyword-remove
                              span.keyword-text Vue JS
                            span.keyword
                              span.keyword-remove
                              span.keyword-text iOS
                            span.keyword
                              span.keyword-remove
                              span.keyword-text Android
                            span.keyword
                              span.keyword-remove
                              span.keyword-text Laravel
                          .clearfix
                    .col-xl-4
                      .submit-field
                        h5 Attachments
                        // Attachments
                        .attachments-container.margin-top-0.margin-bottom-0
                          .attachment-box.ripple-effect
                            span Cover Letter
                            i PDF
                            button.remove-attachment(data-tippy-placement='top', title='Remove')
                          .attachment-box.ripple-effect
                            span Contract
                            i DOCX
                            button.remove-attachment(data-tippy-placement='top', title='Remove')
                        .clearfix
                        // Upload Button
                        .uploadButton.margin-top-0
                          input#upload.uploadButton-input(type='file', accept='image/*, application/pdf', multiple='')
                          label.uploadButton-button.ripple-effect(for='upload') Upload Files
                          span.uploadButton-file-name Maximum file size: 10 MB
                li
                  .row
                    .col-xl-6
                      .submit-field
                        h5 Tagline
                        input.with-border(type='text', value='iOS Expert + Node Dev')
                    .col-xl-6
                      .submit-field
                        h5 Nationality
                        select.selectpicker.with-border(data-size='7', title='Select Job Type', data-live-search='true')
                          option(value='AR') Argentina
                          option(value='AM') Armenia
                          option(value='AW') Aruba
                          option(value='AU') Australia
                          option(value='AT') Austria
                          option(value='AZ') Azerbaijan
                          option(value='BS') Bahamas
                          option(value='BH') Bahrain
                          option(value='BD') Bangladesh
                          option(value='BB') Barbados
                          option(value='BY') Belarus
                          option(value='BE') Belgium
                          option(value='BZ') Belize
                          option(value='BJ') Benin
                          option(value='BM') Bermuda
                          option(value='BT') Bhutan
                          option(value='BG') Bulgaria
                          option(value='BF') Burkina Faso
                          option(value='BI') Burundi
                          option(value='KH') Cambodia
                          option(value='CM') Cameroon
                          option(value='CA') Canada
                          option(value='CV') Cape Verde
                          option(value='KY') Cayman Islands
                          option(value='CO') Colombia
                          option(value='KM') Comoros
                          option(value='CG') Congo
                          option(value='CK') Cook Islands
                          option(value='CR') Costa Rica
                          option(value='CI') Côte d'Ivoire
                          option(value='HR') Croatia
                          option(value='CU') Cuba
                          option(value='CW') Curaçao
                          option(value='CY') Cyprus
                          option(value='CZ') Czech Republic
                          option(value='DK') Denmark
                          option(value='DJ') Djibouti
                          option(value='DM') Dominica
                          option(value='DO') Dominican Republic
                          option(value='EC') Ecuador
                          option(value='EG') Egypt
                          option(value='GP') Guadeloupe
                          option(value='GU') Guam
                          option(value='GT') Guatemala
                          option(value='GG') Guernsey
                          option(value='GN') Guinea
                          option(value='GW') Guinea-Bissau
                          option(value='GY') Guyana
                          option(value='HT') Haiti
                          option(value='HN') Honduras
                          option(value='HK') Hong Kong
                          option(value='HU') Hungary
                          option(value='IS') Iceland
                          option(value='IN') India
                          option(value='ID') Indonesia
                          option(value='NO') Norway
                          option(value='OM') Oman
                          option(value='PK') Pakistan
                          option(value='PW') Palau
                          option(value='PA') Panama
                          option(value='PG') Papua New Guinea
                          option(value='PY') Paraguay
                          option(value='PE') Peru
                          option(value='PH') Philippines
                          option(value='PN') Pitcairn
                          option(value='PL') Poland
                          option(value='PT') Portugal
                          option(value='PR') Puerto Rico
                          option(value='QA') Qatar
                          option(value='RE') Réunion
                          option(value='RO') Romania
                          option(value='RU') Russian Federation
                          option(value='RW') Rwanda
                          option(value='SZ') Swaziland
                          option(value='SE') Sweden
                          option(value='CH') Switzerland
                          option(value='TR') Turkey
                          option(value='TM') Turkmenistan
                          option(value='TV') Tuvalu
                          option(value='UG') Uganda
                          option(value='UA') Ukraine
                          option(value='GB') United Kingdom
                          option(value='US', selected='') United States
                          option(value='UY') Uruguay
                          option(value='UZ') Uzbekistan
                          option(value='YE') Yemen
                          option(value='ZM') Zambia
                          option(value='ZW') Zimbabwe
                    .col-xl-12
                      .submit-field
                        h5 Introduce Yourself
                        textarea.with-border(cols='30', rows='5')
                          | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
        // Dashboard Box
        .col-xl-12
          #test1.dashboard-box
            // Headline
            .headline
              h3
                i.icon-material-outline-lock
                |  Password & Security
            .content.with-padding
              .row
                .col-xl-4
                  .submit-field
                    h5 Current Password
                    input.with-border(type='password')
                .col-xl-4
                  .submit-field
                    h5 New Password
                    input.with-border(type='password')
                .col-xl-4
                  .submit-field
                    h5 Repeat New Password
                    input.with-border(type='password')
                .col-xl-12
                  .checkbox
                    input#two-step(type='checkbox', checked='')
                    label(for='two-step')
                      span.checkbox-icon
                      |  Enable Two-Step Verification via Email
        // Button
        .col-xl-12
          a.button.ripple-effect.big.margin-top-30(href='#') Save Changes
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