<template lang="pug">
div
  //
    Titlebar
    ================================================== 
  #titlebar.gradient
    .container
      .row
        .col-md-12
          h2 Checkout
          // Breadcrumbs
          nav#breadcrumbs.dark
            ul
              li
                a(href='#') Home
              li
                a(href='#') Pricing Plans
              li Checkout

  //| !-- Content
  //| ================================================== 
  // Container
  .container
    .row
      .col-xl-8.col-lg-8.content-right-offset
        // Hedaline
        h3 Billing Cycle
        // Billing Cycle Radios
        .billing-cycle.margin-top-25
          // Radio
          .radio
            input#radio-5(name='radio-payment-type', type='radio', checked='')
            label(for='radio-5')
              span.radio-label
              | 						Billed Monthly
              span.billing-cycle-details
                span.regular-price-tag $49.00 / month
          // Radio
          .radio
            input#radio-6(name='radio-payment-type', type='radio')
            label(for='radio-6')
              span.radio-label
              | 						Billed Yearly
              span.billing-cycle-details
                span.discounted-price-tag $529.20 / year
                span.regular-price-tag.line-through 588.00 / year
        // Hedline
        h3.margin-top-50 Payment Method
        // Payment Methods Accordion
        .payment.margin-top-30
          .payment-tab.payment-tab-active
            .payment-tab-trigger
              input#paypal(checked='', name='cardType', type='radio', value='paypal')
              label(for='paypal') PayPal
              img.payment-logo.paypal(src='https://i.imgur.com/ApBxkXU.png', alt='')
            .payment-tab-content
              p You will be redirected to PayPal to complete payment.
          .payment-tab
            .payment-tab-trigger
              input#creditCart(type='radio', name='cardType', value='creditCard')
              label(for='creditCart') Credit / Debit Card
              img.payment-logo(src='https://i.imgur.com/IHEKLgm.png', alt='')
            .payment-tab-content
              .row.payment-form-row
                .col-md-6
                  .card-label
                    input#nameOnCard(name='nameOnCard', required='', type='text', placeholder='Cardholder Name')
                .col-md-6
                  .card-label
                    input#cardNumber(name='cardNumber', placeholder='Credit Card Number', required='', type='text')
                .col-md-4
                  .card-label
                    input#expiryDate(placeholder='Expiry Month', required='', type='text')
                .col-md-4
                  .card-label
                    label(for='expiryDate') Expiry Year
                    input#expirynDate(placeholder='Expiry Year', required='', type='text')
                .col-md-4
                  .card-label
                    input#cvv(required='', type='text', placeholder='CVV')
        // Payment Methods Accordion / End
        a.button.big.ripple-effect.margin-top-40.margin-bottom-65(href='pages-order-confirmation.html') Proceed Payment
      // Summary
      .col-xl-4.col-lg-4.margin-top-0.margin-bottom-60
        // Summary
        .boxed-widget.summary.margin-top-0
          .boxed-widget-headline
            h3 Summary
          .boxed-widget-inner
            ul
              li
                | Standard Plan 
                span $49.00
              li
                | VAT (20%) 
                span $9.80
              li.total-costs
                | Final Price 
                span $58.80
        // Summary / End
        // Checkbox
        .checkbox.margin-top-30
          input#two-step(type='checkbox')
          label(for='two-step')
            span.checkbox-icon
            |   I agree to the 
            a(href='#') Terms and Conditions
            |  and the 
            a(href='#') Automatic Renewal Terms
  // Container / End

</template>

<script>
// titlebar
// content (this)
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