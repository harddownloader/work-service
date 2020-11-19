<template lang="pug">
div
  //
    Content
    ================================================== 
  #titlebar.gradient
    .container
      .row
        .col-md-12
          h2 Blog
          span Blog Post Page
          // Breadcrumbs
          nav#breadcrumbs.dark
            ul
              li
                a(href='#') Home
              li
                a(href='#') Blog
              li Blog Post
  // Post Content
  .container
    .row
      // Inner Content
      .col-xl-8.col-lg-8
        // Blog Post
        .blog-post.single-post
          // Blog Post Thumbnail
          .blog-post-thumbnail
            .blog-post-thumbnail-inner
              span.blog-item-tag Tips
              img(src='images/blog-04.jpg', alt='')
          // Blog Post Content
          .blog-post-content
            h3.margin-bottom-10 5 Myths That Prevent Job Seekers from Overcoming Failure
            .blog-post-info-list.margin-bottom-20
              a.blog-post-info(href='#') 22 July 2019
              a.blog-post-info(href='#') 5 Comments
            p
              | Nam nisl lacus, dignissim ac tristique ut, scelerisque eu massa. Vestibulum ligula nunc, rutrum in malesuada vitae, tempus sed augue. Curabitur quis lectus quis augue dapibus facilisis. Vivamus tincidunt orci est, in vehicula nisi eleifend ut. Vestibulum sagittis varius orci vitae.
            blockquote.margin-top-20.margin-bottom-20
              | Mauris aliquet ultricies ante, non faucibus ante gravida sed. Sed ultrices pellentesque purus, vulputate volutpat ipsum hendrerit sed neque sed sapien rutrum.
            p
              | In ut odio libero, at vulputate urna. Nulla tristique mi a massa convallis cursus. Nulla eu mi magna. Etiam suscipit commodo gravida. Cras suscipit, quam vitae adipiscing faucibus, risus nibh laoreet odio, a porttitor metus eros ut enim. Morbi augue velit, tempus mattis dignissim nec, porta sed risus. Donec eget magna eu lorem tristique pellentesque eget eu dui. Fusce lacinia tempor malesuada. Ut lacus sapien, placerat a ornare nec, elementum sit amet felis. Maecenas pretium lorem hendrerit eros sagittis fermentum.
            p
              | Phasellus enim magna, varius et commodo ut, ultricies vitae velit. Ut nulla tellus, eleifend euismod pellentesque vel, sagittis vel justo. In libero urna, venenatis sit amet ornare non, suscipit nec risus. Sed consequat justo non mauris pretium at tempor justo sodales. Quisque tincidunt laoreet malesuada. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer vitae ante enim. Fusce sed elit est. Suspendisse sit amet mauris in quam pretium faucibus et aliquam odio.
            // Share Buttons
            .share-buttons.margin-top-25
              .share-buttons-trigger
                i.icon-feather-share-2
              .share-buttons-content
                span
                  | Interesting? 
                  strong Share It!
                ul.share-buttons-icons
                  li
                    a(href='#', data-button-color='#3b5998', title='Share on Facebook', data-tippy-placement='top')
                      i.icon-brand-facebook-f
                  li
                    a(href='#', data-button-color='#1da1f2', title='Share on Twitter', data-tippy-placement='top')
                      i.icon-brand-twitter
                  li
                    a(href='#', data-button-color='#dd4b39', title='Share on Google Plus', data-tippy-placement='top')
                      i.icon-brand-google-plus-g
                  li
                    a(href='#', data-button-color='#0077b5', title='Share on LinkedIn', data-tippy-placement='top')
                      i.icon-brand-linkedin-in
        // Blog Post Content / End
        // Blog Nav
        ul#posts-nav.margin-top-0.margin-bottom-40
          li.next-post
            a(href='#')
              span Next Post
              strong 16 Ridiculously Easy Ways to Find & Keep a Remote Job
          li.prev-post
            a(href='#')
              span Previous Post
              strong 11 Tips to Help You Get New Clients Through Cold Calling
        // Related Posts
        .row
          // Headline
          .col-xl-12
            h3.margin-top-40.margin-bottom-35 Related Posts
          // Blog Post Item
          .col-xl-6
            //- a.blog-compact-item-container(href='pages-blog-post.html')
            nuxt-link.blog-compact-item-container(to="pages-blog-post")
              .blog-compact-item
                img(src='images/blog-02a.jpg', alt='')
                span.blog-item-tag Recruiting
                .blog-compact-item-content
                  ul.blog-post-tags
                    li 29 June 2019
                  h3 How to "Woo" a Recruiter and Land Your Dream Job
                  p
                    | Appropriately empower dynamic leadership skills after business portals. Globally myocardinate interactive.
          // Blog post Item / End
          // Blog Post Item
          .col-xl-6
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
          // Blog post Item / End
          // Related Posts / End
          // Comments
          .row
            .col-xl-12
              section.comments
                h3.margin-top-45.margin-bottom-0
                  | Comments 
                  span.comments-amount (5)
                ul
                  li
                    .avatar
                      img(src='images/user-avatar-placeholder.png', alt='')
                    .comment-content
                      .arrow-comment
                      .comment-by
                        | Kathy Brown
                        span.date 12th, June 2019
                        a.reply(href='#')
                          i.fa.fa-reply
                          |  Reply
                      p
                        | Morbi velit eros, sagittis in facilisis non, rhoncus et erat. Nam posuere tristique sem, eu ultricies tortor imperdiet vitae. Curabitur lacinia neque non metus
                    ul
                      li
                        .avatar
                          img(src='images/user-avatar-placeholder.png', alt='')
                        .comment-content
                          .arrow-comment
                          .comment-by
                            | Tom Smith
                            span.date 12th, June 2019
                            a.reply(href='#')
                              i.fa.fa-reply
                              |  Reply
                          p
                            | Rrhoncus et erat. Nam posuere tristique sem, eu ultricies tortor imperdiet vitae. Curabitur lacinia neque.
                      li
                        .avatar
                          img(src='images/user-avatar-placeholder.png', alt='')
                        .comment-content
                          .arrow-comment
                          .comment-by
                            | Kathy Brown
                            span.date 12th, June 2019
                            a.reply(href='#')
                              i.fa.fa-reply
                              |  Reply
                          p Nam posuere tristique sem, eu ultricies tortor.
                        ul
                          li
                            .avatar
                              img(src='images/user-avatar-placeholder.png', alt='')
                            .comment-content
                              .arrow-comment
                              .comment-by
                                | John Doe
                                span.date 12th, June 2019
                                a.reply(href='#')
                                  i.fa.fa-reply
                                  |  Reply
                              p Great template!
                  li
                    .avatar
                      img(src='images/user-avatar-placeholder.png', alt='')
                    .comment-content
                      .arrow-comment
                      .comment-by
                        | John Doe
                        span.date 15th, May 2015
                        a.reply(href='#')
                          i.fa.fa-reply
                          |  Reply
                      p
                        | Commodo est luctus eget. Proin in nunc laoreet justo volutpat blandit enim. Sem felis, ullamcorper vel aliquam non, varius eget justo. Duis quis nunc tellus sollicitudin mauris.
          // Comments / End
          // Leava a Comment
          .row
            .col-xl-12
              h3.margin-top-35.margin-bottom-30 Add Comment
              // Form
              form#add-comment(method='post')
                .row
                  .col-xl-6
                    .input-with-icon-left.no-border
                      i.icon-material-outline-account-circle
                      input#namecomment.input-text(type='text', name='commentname', placeholder='Name', required='')
                  .col-xl-6
                    .input-with-icon-left.no-border
                      i.icon-material-baseline-mail-outline
                      input#emailaddress.input-text(type='text', name='emailaddress', placeholder='Email Address', required='')
                textarea(name='comment-content', cols='30', rows='5', placeholder='Comment')
              // Button
              button.button.button-sliding-icon.ripple-effect.margin-bottom-40(type='submit', form='add-comment')
                | Add Comment 
                i.icon-material-outline-arrow-right-alt
          // Leava a Comment / End
      // Inner Content / End
      .col-xl-4.col-lg-4.content-left-offset
        .sidebar-container
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
                a.widget-content.active(href='#')
                  img(src='images/blog-02a.jpg', alt='')
                  .widget-text
                    h5 How to "Woo" a Recruiter and Land Your Dream Job
                    span 29 June 2019
              // Post #2
              li
                a.widget-content(href='#')
                  img(src='images/blog-07a.jpg', alt='')
                  .widget-text
                    h5 What It Really Takes to Make $100k Before You Turn 30
                    span 3 June 2019
              // Post #3
              li
                a.widget-content(href='#')
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

</template>

<script>
// content 
// post content 
// spacer
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