<template lang="pug">
// Features Cities
.section.margin-top-65.margin-bottom-65
  .container
    .row
      // Section Headline
      .col-xl-12
        .section-headline.centered.margin-top-0.margin-bottom-45
          h3 Featured Cities
      .col-xl-3.col-md-6
        // Photo Box
        a.photo-box(href='jobs-list-layout-1.html', data-background-image='/images/featured-city-01.jpg')
          .photo-box-content
            h3 San Francisco
            span 376 Jobs
      .col-xl-3.col-md-6
        // Photo Box
        a.photo-box(href='jobs-list-layout-full-page-map.html', data-background-image='/images/featured-city-02.jpg')
          .photo-box-content
            h3 New York
            span 645 Jobs
      .col-xl-3.col-md-6
        // Photo Box
        a.photo-box(href='jobs-grid-layout-full-page.html', data-background-image='/images/featured-city-03.jpg')
          .photo-box-content
            h3 Los Angeles
            span 832 Jobs
      .col-xl-3.col-md-6
        // Photo Box
        a.photo-box(href='jobs-list-layout-2.html', data-background-image='/images/featured-city-04.jpg')
          .photo-box-content
            h3 Miami
            span 513 Jobs
// Features Cities / End

</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    
  })
</script>

<style scoped>

</style>