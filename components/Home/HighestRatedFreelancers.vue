<template lang="pug">
// Highest Rated Freelancers
.section.gray.padding-top-65.padding-bottom-70.full-width-carousel-fix
  .container
    .row
      .col-xl-12
        // Section Headline
        .section-headline.margin-top-0.margin-bottom-25
          h3 Highest Rated Freelancers
          a.headline-link(href='freelancers-grid-layout.html') Browse All Freelancers
      .col-xl-12
        no-ssr
            slick-slide.default-slick-carousel.freelancers-container.freelancers-grid-layout(ref='slick', :options='slickOptions')
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      .verified-badge
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-big-01.jpg', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='single-freelancer-profile.html')
                          | Tom Smith 
                          img.flag(src='/images/flags/gb.svg', alt='', title='United Kingdom', data-tippy-placement='top')
                      span UI/UX Designer
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='5.0')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  London
                      li
                        | Rate 
                        strong $60 / hr
                      li
                        | Job Success 
                        strong 95%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      .verified-badge
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-big-02.jpg', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='#')
                          | David Peterson 
                          img.flag(src='/images/flags/de.svg', alt='', title='Germany', data-tippy-placement='top')
                      span iOS Expert + Node Dev
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='5.0')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  Berlin
                      li
                        | Rate 
                        strong $40 / hr
                      li
                        | Job Success 
                        strong 88%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-placeholder.png', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='#')
                          | Marcin Kowalski 
                          img.flag(src='/images/flags/pl.svg', alt='', title='Poland', data-tippy-placement='top')
                      span Front-End Developer
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='4.9')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  Warsaw
                      li
                        | Rate 
                        strong $50 / hr
                      li
                        | Job Success 
                        strong 100%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      .verified-badge
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-big-03.jpg', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='#')
                          | Sindy Forest 
                          img.flag(src='/images/flags/au.svg', alt='', title='Australia', data-tippy-placement='top')
                      span Magento Certified Developer
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='5.0')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  Brisbane
                      li
                        | Rate 
                        strong $70 / hr
                      li
                        | Job Success 
                        strong 100%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-placeholder.png', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='#')
                          | Sebastiano Piccio 
                          img.flag(src='/images/flags/it.svg', alt='', title='Italy', data-tippy-placement='top')
                      span Laravel Dev
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='4.5')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  Milan
                      li
                        | Rate 
                        strong $80 / hr
                      li
                        | Job Success 
                        strong 89%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
              // Freelancer
              .freelancer
                // Overview
                .freelancer-overview
                  .freelancer-overview-inner
                    // Bookmark Icon
                    span.bookmark-icon
                    // Avatar
                    .freelancer-avatar
                      a(href='single-freelancer-profile.html')
                        img(src='/images/user-avatar-placeholder.png', alt='')
                    // Name
                    .freelancer-name
                      h4
                        a(href='#')
                          | Gabriel Lagueux 
                          img.flag(src='/images/flags/fr.svg', alt='', title='France', data-tippy-placement='top')
                      span WordPress Expert
                    // Rating
                    .freelancer-rating
                      .star-rating(data-rating='5.0')
                // Details
                .freelancer-details
                  .freelancer-details-list
                    ul
                      li
                        | Location 
                        strong
                          i.icon-material-outline-location-on
                          |  Paris
                      li
                        | Rate 
                        strong $50 / hr
                      li
                        | Job Success 
                        strong 100%
                  a.button.button-sliding-icon.ripple-effect(href='single-freelancer-profile.html')
                    | View Profile 
                    i.icon-material-outline-arrow-right-alt
              // Freelancer / End
  // Highest Rated Freelancers / End

  
</template>

<script>
  export default {
    components: { Slick: () => (typeof window !== 'undefined') ? import('vue-slick') : 'undefined' },
    data() {
      return {
        slickOptions: {
          slidesToShow: 3,
          slidesToScroll: 2,
        }
      }
    },
    methods: {},
    mutations: {}
  }
</script>

<style>
  @import 'node_modules/slick-carousel/slick/slick.css';
  .full-width-carousel-fix .default-slick-carousel.slick-initialized .freelancer, .full-width-carousel-fix .blog-carousel.slick-initialized .blog-compact-item-container{
    opacity: 1;
  }
</style>
