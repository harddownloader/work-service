<template lang="pug">
  div
    logo(
      name="Asuxs"
      img="../Asuxs-a7riv3.jpg"
      :rating="5"
    )
    h1 {{ headingH1 }}
    h2 Hello World 1 {{ about_var }}
    logo(
      name="Sony A7RIV"
      img="../sony-a7riv.jpg"
      :rating="9"
    )
    .stats(
      v-for="stat in stats"
      :key="stat.name"
    )
      h3 {{ stat.count }}
      h4 {{ stat.name }}
</template>

<script>
import { mapMutations, mapGetters } from 'vuex'

// import Logo from '~/components/base/Logo.vue'
// import Logo from '~/components/Logo.vue'

export default {
  data: function() {
    return {
      about_var: 3, //this.$store.state.counter,
      headingH1: 3 //this.$store.state.nameApp
    }
  },

  components: {
    Logo
  },

  computed: mapGetters({
    stats: 'projectStatistics/stats'
  }),

  methods: {

  }
}
</script>

<style lang="stulys" scoped>

</style>