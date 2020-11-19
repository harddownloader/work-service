<template lang="pug">
div
  //
    Content
    ================================================== 
  #titlebar.white.margin-bottom-30
    .container
      .row
        .col-md-12
          h2 Blog
          span Featured Posts
          // Breadcrumbs
          nav#breadcrumbs.dark
            ul
              li
                a(href='#') Home
              li Blog
  // Recent Blog Posts
  .section.white.padding-top-0.padding-bottom-60.full-width-carousel-fix
    .container
      .row
        .col-xl-12
          .blog-carousel
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-04a.jpg', alt='')
                span.blog-item-tag Tips
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 20 May 2019
                  h3 5 Myths That Prevent Job Seekers from Overcoming Failure
                  p
                    | Distinctively reengineer revolutionary meta-services and premium architectures intuitive opportunities.
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-05a.jpg', alt='')
                span.blog-item-tag Recruiting
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 28 April 2019
                  h3 12 Dog-Friendly Companies Hiring Now
                  p
                    | Compellingly embrace empowered e-business after user friendly intellectual capital. Interactively front-end.
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-03a.jpg', alt='')
                span.blog-item-tag Marketing
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 10 June 2019
                  h3 11 Tips to Help You Get New Clients Through Cold Calling
                  p
                    | Compellingly embrace empowered e-business after user friendly intellectual capital. Interactively front-end.
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-06a.jpg', alt='')
                span.blog-item-tag Recruiting
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 9 June 2019
                  h3 Follow Up On Job Application With This Template
                  p
                    | Appropriately empower dynamic leadership skills after business portals. Globally myocardinate interactive.
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-07a.jpg', alt='')
                span.blog-item-tag Recruiting
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 3 June 2019
                  h3 What It Really Takes to Make $100k Before You Turn 30
                  p
                    | Appropriately empower dynamic leadership skills after business portals. Globally myocardinate interactive.
  // Recent Blog Posts / End
  // Section
  .section.gray
    .container
      .row
        .col-xl-8.col-lg-8
          // Section Headline
          .section-headline.margin-top-60.margin-bottom-35
            h4 Recent Posts
          // Blog Post
          //- a.blog-post(href='pages-blog-post.html')
          nuxt-link.blog-post(to="pages-blog-post")
            // Blog Post Thumbnail
            .blog-post-thumbnail
              .blog-post-thumbnail-inner
                span.blog-item-tag Tips
                img(src='images/blog-01a.jpg', alt='')
            // Blog Post Content
            .blog-post-content
              span.blog-post-date 22 July 2019
              h3 16 Ridiculously Easy Ways to Find & Keep a Remote Job
              p
                | Efficiently myocardinate market-driven innovation via open-source alignments. Dramatically engage high-payoff infomediaries rather than.
            // Icon
            .entry-icon
          // Blog Post
          //- a.blog-post(href='pages-blog-post.html')
          nuxt-link.blog-post(to="pages-blog-post")
            // Blog Post Thumbnail
            .blog-post-thumbnail
              .blog-post-thumbnail-inner
                span.blog-item-tag Recruiting
                img(src='images/blog-02a.jpg', alt='')
            // Blog Post Content
            .blog-post-content
              span.blog-post-date 29 June 2019
              h3 How to "Woo" a Recruiter and Land Your Dream Job
              p
                | Efficiently myocardinate market-driven innovation via open-source alignments. Dramatically engage high-payoff infomediaries rather than.
          // Blog Post
          //- a.blog-post(href='pages-blog-post.html')
          nuxt-link.blog-post(to="pages-blog-post")
            // Blog Post Thumbnail
            .blog-post-thumbnail
              .blog-post-thumbnail-inner
                span.blog-item-tag Marketing
                img(src='images/blog-03a.jpg', alt='')
            // Blog Post Content
            .blog-post-content
              span.blog-post-date 10 June 2019
              h3 11 Tips to Help You Get New Clients Through Cold Calling
              p
                | Efficiently myocardinate market-driven innovation via open-source alignments. Dramatically engage high-payoff infomediaries rather than.
          // Blog Post
          //- a.blog-post(href='pages-blog-post.html')
          nuxt-link.blog-post(to="pages-blog-post")
            // Blog Post Thumbnail
            .blog-post-thumbnail
              .blog-post-thumbnail-inner
                span.blog-item-tag Tips
                img(src='images/blog-04a.jpg', alt='')
            // Blog Post Content
            .blog-post-content
              span.blog-post-date 5 June 2019
              h3 5 Myths That Prevent Job Seekers from Overcoming Failure
              p
                | Efficiently myocardinate market-driven innovation via open-source alignments. Dramatically engage high-payoff infomediaries rather than.
          // Pagination
          .clearfix
          .row
            .col-md-12
              // Pagination
              .pagination-container.margin-top-10.margin-bottom-20
                nav.pagination
                  ul
                    li
                      a.current-page.ripple-effect(href='#') 1
                    li
                      a.ripple-effect(href='#') 2
                    li
                      a.ripple-effect(href='#') 3
                    li.pagination-arrow
                      a.ripple-effect(href='#')
                        i.icon-material-outline-keyboard-arrow-right
          // Pagination / End
        .col-xl-4.col-lg-4.content-left-offset
          .sidebar-container.margin-top-65
            // Location
            .sidebar-widget.margin-bottom-40
              .input-with-icon
                input#autocomplete-input(type='text', placeholder='Search')
                i.icon-material-outline-search
            // Widget
            .sidebar-widget
              h3 Trending Posts
              ul.widget-tabs
                // Post #1
                li
                  //- a.widget-content.active(href='pages-blog-post.html')
                  nuxt-link.widget-content.active(to="pages-blog-post")
                    img(src='images/blog-02a.jpg', alt='')
                    .widget-text
                      h5 How to "Woo" a Recruiter and Land Your Dream Job
                      span 29 June 2019
                // Post #2
                li
                  //- a.widget-content(href='pages-blog-post.html')
                  nuxt-link.widget-content(to="pages-blog-post")
                    img(src='images/blog-07a.jpg', alt='')
                    .widget-text
                      h5 What It Really Takes to Make $100k Before You Turn 30
                      span 3 June 2019
                // Post #3
                li
                  //- a.widget-content(href='pages-blog-post.html')
                  nuxt-link.widget-content(to="pages-blog-post")
                    img(src='images/blog-04a.jpg', alt='')
                    .widget-text
                      h5 5 Myths That Prevent Job Seekers from Overcoming Failure
                      span 5 June 2019
            // Widget / End
            // Widget
            .sidebar-widget
              h3 Social Profiles
              .freelancer-socials.margin-top-25
                ul
                  li
                    a(href='#', title='Dribbble', data-tippy-placement='top')
                      i.icon-brand-dribbble
                  li
                    a(href='#', title='Twitter', data-tippy-placement='top')
                      i.icon-brand-twitter
                  li
                    a(href='#', title='Behance', data-tippy-placement='top')
                      i.icon-brand-behance
                  li
                    a(href='#', title='GitHub', data-tippy-placement='top')
                      i.icon-brand-github
            // Widget
            .sidebar-widget
              h3 Tags
              .task-tags
                a(href='#')
                  span employer
                a(href='#')
                  span recruiting
                a(href='#')
                  span work
                a(href='#')
                  span salary
                a(href='#')
                  span tips
                a(href='#')
                  span income
                a(href='#')
                  span application
    // Spacer
    .padding-top-40
    // Spacer
  // Section / End

</template>

<script>
// content
// recent blog posts 
// section

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