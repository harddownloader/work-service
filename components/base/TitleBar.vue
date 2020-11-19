<template lang="pug">
//
  Titlebar
  ================================================== 
#titlebar.gradient
  .container
    .row
      .col-md-12
        //- h2 Browse Companies
        h2 titlebar
        //- h2 {{ title }}
        // Breadcrumbs
        nav#breadcrumbs.dark
          ul
            //li(v-for='(item, i) in crumbs', :key='i', :class='item.classes')
              nuxt-link(:to='item.path') {{ $t(item.name) }}
</template>

<script>
  export default {
    /*locale: 'ru',
    props: {
      title: String,
      // breadcrumbs: Array
    },
    computed: {
      crumbs() {
        const crumbs = []
        this.$route.matched.map((item, i, { length }) => {
          const crumb = {}
          crumb.path = item.path
          crumb.name = this.$i18n.t('route.' + (item.name || item.path))

          // is last item?
          if (i === length - 1) {
            // is param route? .../.../:id
            if (item.regex.keys.length > 0) {
              crumbs.push({
                path: item.path.replace(/\/:[^/:]*$/, ''),
                name: this.$i18n.t('route.' + item.name.replace(/-[^-]*$/, ''))
              })
              crumb.path = this.$route.path
              crumb.name = this.$i18n.t('route.' + this.$route.name, [
                crumb.path.match(/[^/]*$/)[0]
              ])
            }
            crumb.classes = 'is-active'
          }

          crumbs.push(crumb)
        })

        return crumbs
      }
    }*/
  }
</script>

<style lang="stylus" scoped>

</style>