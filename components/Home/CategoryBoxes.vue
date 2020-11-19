<template lang="pug">
//
  Content
  ==================================================
// Category Boxes
.section.margin-top-65
  .container
    .row
      .col-xl-12
        .section-headline.centered.margin-bottom-15
          h3 Popular Job Categories
        // Category Boxes Container
        .categories-container
          // Category Box
          a.category-box(href='jobs-grid-layout-full-page.html')
            .category-box-icon
              i.icon-line-awesome-file-code-o
            .category-box-counter 612
            .category-box-content
              h3 Web & Software Dev
              p Software Engineer, Web / Mobile Developer & More
          // Category Box
          a.category-box(href='jobs-list-layout-full-page-map.html')
            .category-box-icon
              i.icon-line-awesome-cloud-upload
            .category-box-counter 113
            .category-box-content
              h3 Data Science & Analitycs
              p Data Specialist / Scientist, Data Analyst & More
          // Category Box
          a.category-box(href='jobs-list-layout-full-page-map.html')
            .category-box-icon
              i.icon-line-awesome-suitcase
            .category-box-counter 186
            .category-box-content
              h3 Accounting & Consulting
              p Auditor, Accountant, Fnancial Analyst & More
          // Category Box
          a.category-box(href='jobs-list-layout-1.html')
            .category-box-icon
              i.icon-line-awesome-pencil
            .category-box-counter 298
            .category-box-content
              h3 Writing & Translations
              p Copywriter, Creative Writer, Translator & More
          // Category Box
          a.category-box(href='jobs-list-layout-2.html')
            .category-box-icon
              i.icon-line-awesome-pie-chart
            .category-box-counter 549
            .category-box-content
              h3 Sales & Marketing
              p Brand Manager, Marketing Coordinator & More
          // Category Box
          a.category-box(href='jobs-list-layout-1.html')
            .category-box-icon
              i.icon-line-awesome-image
            .category-box-counter 873
            .category-box-content
              h3 Graphics & Design
              p Creative Director, Web Designer & More
          // Category Box
          a.category-box(href='jobs-list-layout-2.html')
            .category-box-icon
              i.icon-line-awesome-bullhorn
            .category-box-counter 125
            .category-box-content
              h3 Digital Marketing
              p Darketing Analyst, Social Profile Admin & More
          // Category Box
          a.category-box(href='jobs-grid-layout-full-page.html')
            .category-box-icon
              i.icon-line-awesome-graduation-cap
            .category-box-counter 445
            .category-box-content
              h3 Education & Training
              p Advisor, Coach, Education Coordinator & More
// Category Boxes / End

</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    
  })
</script>

<style scoped>

</style>