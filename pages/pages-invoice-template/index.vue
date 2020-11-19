<template lang="pug">
div
  // Print Button
  .print-button-container
    a.print-button(href='javascript:window.print()') Print this invoice
  // Invoice
  #invoice
    // Header
    .row
      .col-xl-6
        #logo
          img(src='images/logo.png', alt='')
      .col-xl-6
        p#details
          strong Order:
          |  #00124 
          br
          strong Issued:
          |  20/08/2019 
          br
          | 				Due 7 days from date of issue
    // Client & Supplier
    .row
      .col-xl-12
        h2 Invoice
      .col-xl-6
        strong.margin-bottom-5 Supplier
        p
          | Hireo Ltd. 
          br
          | 				21 St Andrews Lane 
          br
          | 				London, CF44 6ZL, UK 
          br
      .col-xl-6
        strong.margin-bottom-5 Customer
        p
          | John Doe 
          br
          | 				36 Edgewater Street 
          br
          | 				Melbourne, 2540, Australia 
          br
    // Invoice
    .row
      .col-xl-12
        table.margin-top-20
          tbody
            tr
              th Description
              th Price
              th VAT (20%)
              th Total
            tr
              td Standard Plan
              td $49.00
              td $9.80
              td $58.80
      .col-xl-4.col-xl-offset-8
        table#totals
          tbody
            tr
              th Total Due
              th
                span $58.80
    // Footer
    .row
      .col-xl-12
        ul#footer
          li
            span www.example.com
          li office@example.com
          li (123) 123-456

</template>

<script>
// print btn
// invoice 
  export default {
    layout: 'ForPrint', 
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