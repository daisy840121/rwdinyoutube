<template lang="pug">
div
  h1 對不起出錯啦～～
  img(:src='src')
</template>
<script>
export default{
  props:['error'],
  layout:'error_layout',
  data() {
    return {
      src: 'https://mailbox.mnd.gov.tw/img/Error404-4_03.png' 
    }
}}
</script>
