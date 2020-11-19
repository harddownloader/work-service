<template lang="pug">
div
  
  //Intro Banner==================================================
  // add class "disable-gradient" to enable consistent background overlay
  IntroBanner

  CategoryBoxes

  FeaturesJobs

  FeaturesJobs_2

  FeaturesCities

  HighestRatedFreelancers

  MembershipPlans

  PhotoSection

  RecentBlogPosts

  Partners

</template>

<script>

// import Logo from '~/components/base/Logo.vue'

import IntroBanner from '~/components/Home/IntroBanner.vue'
import CategoryBoxes from '~/components/Home/CategoryBoxes.vue'
import FeaturesJobs from '~/components/Home/FeaturesJobs.vue'
import FeaturesCities from '~/components/Home/FeaturesCities.vue'
import HighestRatedFreelancers from '~/components/Home/HighestRatedFreelancers.vue'
import MembershipPlans from '~/components/Home/MembershipPlans.vue'

import PhotoSection from '~/components/Home/PhotoSection.vue'
import FeaturesJobs_2 from "~/components/Home/FeaturesJobs_2.vue"

import RecentBlogPosts from "~/components/Home/RecentBlogPosts.vue"
import Partners from "~/components/Home/Partners.vue"


export default {
  layout: 'Simple',
  components: {
    
    IntroBanner,
    CategoryBoxes,
    FeaturesJobs,
    FeaturesJobs_2,
    FeaturesCities,
    HighestRatedFreelancers,
    MembershipPlans,
    PhotoSection,
    RecentBlogPosts,
    Partners
    // Logo
  }
}
</script>

<style lang="stylus">

</style>
