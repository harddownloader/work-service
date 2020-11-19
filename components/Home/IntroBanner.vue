<template lang="pug">

.intro-banner(data-background-image='/images/hero.jpg')
  .container
    // Intro Headline
    .row
      .col-md-12
        .banner-headline
          h3
            strong Hire experts or be hired for any job, any time.
            br
            span
              | Thousands of small businesses use 
              strong.color Hireo
              |  to turn their ideas into reality.
    // Search Bar
    .row
      .col-md-12
        .intro-banner-search-form.margin-top-95
          // Search Field
          .intro-search-field.with-autocomplete
            label.field-title.ripple-effect(for='autocomplete-input') Where?
            .input-with-icon
              input#autocomplete-input(type='text', placeholder='Online Job')
              i.icon-material-outline-location-on
          // Search Field
          .intro-search-field
            label.field-title.ripple-effect(for='intro-keywords') What you need done?
            //- input#intro-keywords(type='text', placeholder='e.g. build me a website')
            multiselect.selectpicker.default(
              v-model="value_city",
              :options="options_city",
              :searchable="false",
              :close-on-select="false",
              :show-labels="false"
              placeholder="All Cities"
            )
          // Search Field
          .intro-search-field
            multiselect.selectpicker.default(
              v-model="value_cat",
              :options="options_cat",
              :searchable="false",
              :close-on-select="false",
              :show-labels="false"
              placeholder="All Categories"
            )
            //select.selectpicker.default(multiple='', data-selected-text-format='count', data-size='7', title='All Categories')
              option Admin Support
              option Customer Service
              option Data Analytics
              option Design & Creative
              option Legal
              option Software Developing
              option IT & Networking
              option Writing
              option Translation
              option Sales & Marketing
          // Button
          .intro-search-button
            button.button.ripple-effect(onclick="window.location.href='freelancers-grid-layout-full-page.html'") Search

        //.intro-banner-search-form.margin-top-95
          // Search Field
          .intro-search-field.with-autocomplete
            label.field-title.ripple-effect(for='autocomplete-input') Where?
            .input-with-icon
              input#autocomplete-input(type='text', placeholder='Online Job')
              i.icon-material-outline-location-on
          // Search Field
          .intro-search-field
            label.field-title.ripple-effect(for='intro-keywords') What job you want?
            input#intro-keywords(type='text', placeholder='Job Title or Keywords')
          // Button
          .intro-search-button
            button.button.ripple-effect(onclick="window.location.href='jobs-list-layout-full-page-map.html'") Search
    // Stats
    .row
      .col-md-12
        ul.intro-stats.margin-top-45.hide-under-992px
          li
            strong.counter 1,586
            span Jobs Posted
          li
            strong.counter 3,543
            span Tasks Posted
          li
            strong.counter 1,232
            span Freelancers

</template>

<script>
  // import Vue from 'vue'
  import Multiselect from 'vue-multiselect'

  export default {
     components: { Multiselect },
     data () {
      return {
        
        value_city: null,
        options_city: [
          "Kyiv",
          "Kharkiv",
          "Odessa",
          "Dnipro",
          "Donetsk",
          "Zaporizhia",
          "Lviv",
          "Mykolaiv",
          "Mariupol",
          "Luhansk"
        ],

        value_cat: null,
        options_cat: [
          "Admin Support",
          "Customer Service",
          "Data Analytics",
          "Design & Creative",
          "Legal",
          "Software Developing",
          "IT & Networking",
          "Writing",
          "Translation",
          "Sales & Marketing"
        ],
        
      }
    }
  }
</script>

<style src="vue-multiselect/dist/vue-multiselect.min.css"></style>

<style lang="stylus" scoped>

</style>