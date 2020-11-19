<template lang="pug">
div
  //- titlebar
  TitleBar(
    title="404 Not Found",
    
  )

  //- content
  //
    Page Content
    ==================================================
  // Container
  .container
    .row
      .col-xl-12
        section#not-found.center.margin-top-50.margin-bottom-25
          h2
            | 404 
            i.icon-line-awesome-question-circle
          p We're sorry, but the page you were looking for doesn't exist
        .row
          .col-xl-8.offset-xl-2
            .intro-banner-search-form.not-found-search.margin-bottom-50
              // Search Field
              .intro-search-field
                input#intro-keywords(type='text', placeholder='What Are You Looking For?')
              // Button
              .intro-search-button
                button.button.ripple-effect Search
  // Container / End


  .margin-top-70
  //- <div class="container">
  //-   <h1 v-if="error.statusCode === 404">Страница не найдена</h1>
  //-   <h1 v-else>Произошла ошибка</h1>
  //-   <nuxt-link to="/">Вернуться на главную</nuxt-link>
  //- </div>
</template>

<script>
// import Header from '~/components/base/Header.vue'
// import Footer from '~/components/base/Footer.vue'
import TitleBar from '~/components/base/TitleBar.vue'

export default {
  props: ['error'],
  components: {
    // Header,
    TitleBar,
    // Footer
  }
}
</script>

<style lang="stylus" scoped>
  @import '@/assets/css/icons.css'
  @import '@/assets/css/style-main.css'
  @import '@/assets/css/colors/blue.css'
</style>