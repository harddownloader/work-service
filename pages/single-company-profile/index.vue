<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  .single-page-header(data-background-image='images/single-company.jpg')
    .container
      .row
        .col-md-12
          .single-page-header-inner
            .left-side
              .header-image
                img(src='/images/browse-companies-03.png', alt='')
              .header-details
                h3
                  | Acodia 
                  span Software House
                ul
                  li
                    .star-rating(data-rating='4.9')
                  li
                    img.flag(src='/images/flags/de.svg', alt='')
                    |  Germany
                  li
                    .verified-badge-with-title Verified
            .right-side
              // Breadcrumbs
              nav#breadcrumbs.white
                ul
                  li
                    a(href='#') Home
                  li
                    a(href='#') Browse Companies
                  li Acodia

  //
    Page Content
    ================================================== 
  .container
    .row
      // Content
      .col-xl-8.col-lg-8.content-right-offset
        .single-page-section
          h3.margin-bottom-25 About Company
          p
            | Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.
          p
            | Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.
        // Boxed List
        .boxed-list.margin-bottom-60
          .boxed-list-headline
            h3
              i.icon-material-outline-business-center
              |  Open Positions
          .listings-container.compact-list-layout
            // Job Listing
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Details
                .job-listing-description
                  h3.job-listing-title Python Developer
                  // Job Listing Footer
                  .job-listing-footer
                    ul
                      li
                        i.icon-material-outline-location-on
                        |  Berlin
                      li
                        i.icon-material-outline-business-center
                        |  Full Time
                      li
                        i.icon-material-outline-access-time
                        |  2 days ago
              // Bookmark
              span.bookmark-icon
            // Job Listing
            a.job-listing(href='single-job-page.html')
              // Job Listing Details
              .job-listing-details
                // Details
                .job-listing-description
                  h3.job-listing-title Junior Full Stack Developer
                  // Job Listing Footer
                  .job-listing-footer
                    ul
                      li
                        i.icon-material-outline-location-on
                        |  Berlin
                      li
                        i.icon-material-outline-business-center
                        |  Full Time
                      li
                        i.icon-material-outline-access-time
                        |  2 days ago
              // Bookmark
              span.bookmark-icon
        // Boxed List / End
        // Boxed List
        .boxed-list.margin-bottom-60
          .boxed-list-headline
            h3
              i.icon-material-outline-thumb-up
              |  Reviews
          ul.boxed-list-ul
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | Doing things the right way 
                    span Anonymous Employee
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  August 2019
                  .item-description
                    p
                      | Great company and especially ideal for the career-minded individual. The company is large enough to offer a variety of jobs in all kinds of interesting locations. Even if you never change roles, your job changes and evolves as the company grows, keeping things fresh.
            li
              .boxed-list-item
                // Content
                .item-content
                  h4
                    | Outstanding Work Environment 
                    span Anonymous Employee
                  .item-details.margin-top-10
                    .star-rating(data-rating='5.0')
                    .detail-item
                      i.icon-material-outline-date-range
                      |  May 2019
                  .item-description
                    p
                      | They do business with integrity and rational thinking. Overall, it's an excellent place to work, with products that are winning in the marketplace.
          .centered-button.margin-top-35
            a.popup-with-zoom-anim.button.button-sliding-icon(href='#small-dialog')
              | Leave a Review 
              i.icon-material-outline-arrow-right-alt
        // Boxed List / End
      // Sidebar
      .col-xl-4.col-lg-4
        .sidebar-container
          // Location
          .sidebar-widget
            h3 Location
            #single-job-map-container
              #singleListingMap(data-latitude='52.520007', data-longitude='13.404954', data-map-icon='im im-icon-Hamburger')
              a#streetView(href='#') Street View
          // Widget
          .sidebar-widget
            h3 Social Profiles
            .freelancer-socials.margin-top-25
              ul
                li
                  a(href='#', title='Dribbble', data-tippy-placement='top')
                    i.icon-brand-dribbble
                li
                  a(href='#', title='Twitter', data-tippy-placement='top')
                    i.icon-brand-twitter
                li
                  a(href='#', title='Behance', data-tippy-placement='top')
                    i.icon-brand-behance
                li
                  a(href='#', title='GitHub', data-tippy-placement='top')
                    i.icon-brand-github
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