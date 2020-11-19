<template lang="pug">
  // Wrapper
  #wrapper
    Header(layout="dashboard")
    .clearfix
    // Header Container / End

    //- TitleBar

    nuxt
    
    //- Footer
    
</template>

<style lang="stylus" scoped>
  @import '@/assets/css/icons.css'
  @import '@/assets/css/style-main.css'
  @import '@/assets/css/colors/blue.css'
</style>

<script>
import Vue from 'vue'
import Header from '~/components/base/Header.vue'
// import Footer from '~/components/base/Footer.vue'

// import TitleBar from '~/components/base/TitleBar.vue'

export default Vue.extend({

  components: {
    Header,
    // TitleBar,
    // Footer
  }

})
</script>