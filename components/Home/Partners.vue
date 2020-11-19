<template lang="pug">
.section.border-top.padding-top-45.padding-bottom-45
  // Logo Carousel
  .container
    .row
      .col-xl-12
        // Carousel
        .col-md-12
          no-ssr
            slick-slide.logo-carousel(ref='slick', :options='slickOptions')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-01.png', alt='')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-02.png', alt='')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-03.png', alt='')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-04.png', alt='')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-05.png', alt='')
              .carousel-item
                a(href='http://acmelogos.com/', target='_blank', title='http://acmelogos.com/')
                  img(src='/images/logo-carousel-06.png', alt='')
        // Carousel / End
  //.container
    no-ssr
      slick-slide.carousel-item(ref='slick', :options='slickOptions')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')
        a(href='http://placehold.it/2000x1000')
          img(src='http://placehold.it/2000x1000', alt='')


      


</template>

<script>


 export default {
    components: { Slick: () => (typeof window !== 'undefined') ? import('vue-slick') : 'undefined' },
    data() {
      return {
        slickOptions: {
          slidesToShow: 4,
          slidesToScroll: 4,
        }
      }
    }
  }
</script>

<style >
  @import 'node_modules/slick-carousel/slick/slick.css';
</style>