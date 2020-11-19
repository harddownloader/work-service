<template lang="pug">
div
  TitleBar(title="Browse Companies")
  //
    Page Content
    ================================================== 
  .container
    .row
      .col-xl-12
        .letters-list
          a.current(href='#') A
          a(href='#') B
          a(href='#') C
          a(href='#') D
          a(href='#') E
          a(href='#') F
          a(href='#') G
          a(href='#') H
          a(href='#') I
          a(href='#') J
          a(href='#') K
          a(href='#') L
          a(href='#') M
          a(href='#') N
          a(href='#') O
          a(href='#') P
          a(href='#') Q
          a(href='#') R
          a(href='#') S
          a(href='#') T
          a(href='#') U
          a(href='#') V
          a(href='#') W
          a(href='#') X
          a(href='#') Y
          a(href='#') Z
      .col-xl-12
        .companies-list
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/company-logo-placeholder.png', alt='')
              h4 Acra
              .star-rating(data-rating='3.5')
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/browse-companies-02.png', alt='')
              h4 Acue
              .star-rating(data-rating='5.0')
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/browse-companies-04.png', alt='')
              h4 Acorta
              span.company-not-rated Minimum of 3 votes required
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/company-logo-placeholder.png', alt='')
              h4 Acuneol
              span.company-not-rated Minimum of 3 votes required
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/browse-companies-03.png', alt='')
              h4 Acodia
              .star-rating(data-rating='4.9')
          a.company(href='single-company-profile.html')
            .company-inner-alignment
              span.company-logo
                img(src='images/company-logo-placeholder.png', alt='')
              h4 Acagic
              span.company-not-rated Minimum of 3 votes required
  .margin-top-70

</template>

<script>
  import TitleBar from '~/components/base/TitleBar.vue'
  export default {
    layout: 'Simple',
    components: {
      TitleBar
    }
  }
</script>

<style lang="stylus" scoped>

</style>