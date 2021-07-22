<template lang="pug">
<div>
  header.header
    nav
      ul.nav_wrap
        li
          b-icon.nav_icon_burger(v-b-toggle.sidebar-1, icon="justify")
          Sideber
          img.nav_logo_img(src="logo.png")
        li
          input.search_input(type="text", placeholder="搜尋")
        li
          b-icon.nav_icon(icon="search") 
          img.nav_user_img(src="user.jpg")
    nav
      ul.nav_tags
        li(v-for="item in tags") 
          b-button.nav_tags_btn {{ item.title }}
Nuxt
footer
  ul.footer
    li
      b-icon.footer_icon(icon="house-door")
      p Home
    li
      b-icon.footer_icon(icon="hand-thumbs-up")
      p Trending
    li
      b-icon.footer_icon(icon="play-btn")
      p Subscriptions
    li
      b-icon.footer_icon(icon="bookmark-star")
      p Library
</div>               
</template>
  
<script>
import Sideber from "../components/Sideber.vue";
export default {
  data() {
    return {
      tags: [
        { title: "All" },
        { title: "Music" },
        { title: "One Piece" },
        { title: "Anime" },
        { title: "Love songs" },
        { title: "baseball" },
        { title: "basketball" },
        { title: "Cooking show" },
        { title: "Live broadcast" },
        { title: "Newest upload" },
        { title: "Watched" },
      ],
    };
  },
  components: {
    Sideber,
  },
};
</script>