<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  .single-page-header(data-background-image='images/single-task.jpg')
    .container
      .row
        .col-md-12
          .single-page-header-inner
            .left-side
              .header-image
                a(href='single-company-profile.html')
                  img(src='images/browse-companies-02.png', alt='')
              .header-details
                h3 Food Delivery Mobile Application
                h5 About the Employer
                ul
                  li
                    a(href='single-company-profile.html')
                      i.icon-material-outline-business
                      |  Acue
                  li
                    .star-rating(data-rating='5.0')
                  li
                    img.flag(src='images/flags/de.svg', alt='')
                    |  Germany
                  li
                    .verified-badge-with-title Verified
            .right-side
              .salary-box
                .salary-type Project Budget
                .salary-amount $2,500 - $4,500

  //
    Page Content
    ================================================== 
  .container
    .row
      // Content
      .col-xl-8.col-lg-8.content-right-offset
        // Description
        .single-page-section
          h3.margin-bottom-25 Project Description
          p
            | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
          p
            | Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.
          p
            | Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.
        // Atachments
        .single-page-section
          h3 Attachments
          .attachments-container
            a.attachment-box.ripple-effect(href='#')
              span Project Brief
              i PDF
        // Skills
        .single-page-section
          h3 Skills Required
          .task-tags
            span iOS
            span Android
            span mobile apps
            span design
        .clearfix
        // Freelancers Bidding
        .boxed-list.margin-bottom-60
          .boxed-list-headline
            h3
              i.icon-material-outline-group
              |  Freelancers Bidding
          ul.boxed-list-ul
            li
              .bid
                // Avatar
                .bids-avatar
                  .freelancer-avatar
                    .verified-badge
                    a(href='single-freelancer-profile.html')
                      img(src='images/user-avatar-big-01.jpg', alt='')
                // Content
                .bids-content
                  // Name
                  .freelancer-name
                    h4
                      a(href='single-freelancer-profile.html')
                        | Tom Smith 
                        img.flag(src='images/flags/gb.svg', alt='', title='United Kingdom', data-tippy-placement='top')
                    .star-rating(data-rating='4.9')
                // Bid
                .bids-bid
                  .bid-rate
                    .rate $4,400
                    span in 7 days
            li
              .bid
                // Avatar
                .bids-avatar
                  .freelancer-avatar
                    .verified-badge
                    a(href='single-freelancer-profile.html')
                      img(src='images/user-avatar-big-02.jpg', alt='')
                // Content
                .bids-content
                  // Name
                  .freelancer-name
                    h4
                      a(href='single-freelancer-profile.html')
                        | David Peterson 
                        img.flag(src='images/flags/de.svg', alt='', title='Germany', data-tippy-placement='top')
                    .star-rating(data-rating='4.2')
                // Bid
                .bids-bid
                  .bid-rate
                    .rate $2,200
                    span in 14 days
            li
              .bid
                // Avatar
                .bids-avatar
                  .freelancer-avatar
                    a(href='single-freelancer-profile.html')
                      img(src='images/user-avatar-placeholder.png', alt='')
                // Content
                .bids-content
                  // Name
                  .freelancer-name
                    h4
                      a(href='single-freelancer-profile.html')
                        | Marcin Kowalski 
                        img.flag(src='images/flags/pl.svg', alt='', title='Poland', data-tippy-placement='top')
                    span.not-rated Minimum of 3 votes required
                // Bid
                .bids-bid
                  .bid-rate
                    .rate $3,800
                    span In 20 days
            li
              .bid
                // Avatar
                .bids-avatar
                  .freelancer-avatar
                    a(href='single-freelancer-profile.html')
                      img(src='images/user-avatar-placeholder.png', alt='')
                // Content
                .bids-content
                  // Name
                  .freelancer-name
                    h4
                      a(href='single-freelancer-profile.html')
                        | Sebastiano Piccio 
                        img.flag(src='images/flags/it.svg', alt='', title='Italy', data-tippy-placement='top')
                    .star-rating(data-rating='4.5')
                // Bid
                .bids-bid
                  .bid-rate
                    .rate $3,400
                    span In 10 days
      // Sidebar
      .col-xl-4.col-lg-4
        .sidebar-container
          .countdown.green.margin-bottom-35 6 days, 23 hours left
          .sidebar-widget
            .bidding-widget
              .bidding-headline
                h3 Bid on this job!
              .bidding-inner
                // Headline
                span.bidding-detail
                  | Set your 
                  strong minimal rate
                // Price Slider
                .bidding-value
                  | $
                  span#biddingVal
                input.bidding-slider(type='text', value='', data-slider-handle='custom', data-slider-currency='$', data-slider-min='2500', data-slider-max='4500', data-slider-value='auto', data-slider-step='50', data-slider-tooltip='hide')
                // Headline
                span.bidding-detail.margin-top-30
                  | Set your 
                  strong delivery time
                // Fields
                .bidding-fields
                  .bidding-field
                    // Quantity Buttons
                    .qtyButtons
                      .qtyDec
                      input(type='text', name='qtyInput', value='1')
                      .qtyInc
                  .bidding-field
                    select.selectpicker.default
                      option(selected='') Days
                      option Hours
                // Button
                button#snackbar-place-bid.button.ripple-effect.move-on-hover.full-width.margin-top-30
                  span Place a Bid
              .bidding-signup
                | Don't have an account? 
                a.register-tab.sign-in.popup-with-zoom-anim(href='#sign-in-dialog') Sign Up
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

  .margin-top-15
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