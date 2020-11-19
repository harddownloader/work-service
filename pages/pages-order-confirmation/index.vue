<template lang="pug">
// Container
.container
  .row
    .col-md-12
      .order-confirmation-page
        .breathing-icon
          i.icon-feather-check
        h2.margin-top-30 Thank you for your order!
        p Your payment has been processed successfully.
        a.button.ripple-effect-dark.button-sliding-icon.margin-top-30(href='pages-invoice-template.html')
          | View Invoice 
          i.icon-material-outline-arrow-right-alt
// Container / End

</template>

<script>
// content который titlebar
// container(this)
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