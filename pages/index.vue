<template lang="pug">
.content
    ul.wrap
      li.item(v-for='item in data')
        img.item_Img(:src='item.img')
        .txt
          .user_img
            img.txt_img(src='user.jpg')
          .txt_title
            h3.txt_h3 {{ item.title }}
              b-icon.den(icon='three-dots-vertical')
            p.txt_p {{ item.author }}
              br/ 觀看次數：{{ item.num }} • {{ item.day }} 
</template>
<script>
export default {
  async asyncData({ $axios }) {
    const data = await $axios.$get("http://localhost:8888/objects");
    return { data };
  }
};
</script>


  
