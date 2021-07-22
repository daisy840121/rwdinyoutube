<template lang="pug">
b-sidebar#sidebar-1(shadow='')
  .px-3.py-2
    ul.burger
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='house-door') 
          | &emsp;首頁
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='search')
          | &emsp;搜索
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='bookmark-heart')
          | &emsp;訂閱
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='play-btn')
          | &emsp;媒體
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='arrow-counterclockwise')
          | &emsp;紀錄
      li.tagItem
        a.tagLink(href='#')
          b-icon.tagIcon(icon='house-door')
          | &emsp;影片
</template>
