<template lang="pug">
//
  Page Content
  ================================================== 
.container
  .row
    .col-xl-12
      // Billing Cycle
      .billing-cycle-radios.margin-bottom-70
        .radio.billed-monthly-radio
          input#radio-5(name='radio-payment-type', type='radio', checked='')
          label(for='radio-5')
            span.radio-label
            |  Billed Monthly
        .radio.billed-yearly-radio
          input#radio-6(name='radio-payment-type', type='radio')
          label(for='radio-6')
            span.radio-label
            |  Billed Yearly 
            span.small-label Save 10%
      // Pricing Plans Container
      .pricing-plans-container
        // Plan
        .pricing-plan
          h3 Basic Plan
          p.margin-top-10 One time fee for one listing or task highlighted in search results.
          .pricing-plan-label.billed-monthly-label
            strong $19
            | / monthly
          .pricing-plan-label.billed-yearly-label
            strong $205
            | / yearly
          .pricing-plan-features
            strong Features of Basic Plan
            ul
              li 1 Listing
              li 30 Days Visibility
              li Highlighted in Search Results
          a.button.full-width.margin-top-20(href='pages-checkout-page.html') Buy Now
        // Plan
        .pricing-plan.recommended
          .recommended-badge Recommended
          h3 Standard Plan
          p.margin-top-10 One time fee for one listing or task highlighted in search results.
          .pricing-plan-label.billed-monthly-label
            strong $49
            | / monthly
          .pricing-plan-label.billed-yearly-label
            strong $529
            | / yearly
          .pricing-plan-features
            strong Features of Standard Plan
            ul
              li 5 Listings
              li 60 Days Visibility
              li Highlighted in Search Results
          a.button.full-width.margin-top-20(href='pages-checkout-page.html') Buy Now
        // Plan
        .pricing-plan
          h3 Extended Plan
          p.margin-top-10 One time fee for one listing or task highlighted in search results.
          .pricing-plan-label.billed-monthly-label
            strong $99
            | / monthly
          .pricing-plan-label.billed-yearly-label
            strong $1069
            | / yearly
          .pricing-plan-features
            strong Features of Extended Plan
            ul
              li Unlimited Listings Listing
              li 90 Days Visibility
              li Highlighted in Search Results
          a.button.full-width.margin-top-20(href='pages-checkout-page.html') Buy Now

</template>

<script>

// titlebar
// page content(this)
// margin-top-80 (т.е. spacer)

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