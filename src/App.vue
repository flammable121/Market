<template>
  <div>
    <header-menu class="header-menu"/>
    <full-screen-baner class="full-screen-baner"/>
    <categories-board class="categories-board"/>
    <form-news class="form-news"/>
    <footer-info class="footer"/>
  </div>
</template>

<script setup>
  import FullScreenBaner from './components/FullScreenBaner.vue'
  import HeaderMenu from './components/HeaderMenu.vue'
  import CategoriesBoard from './components/CategoriesBoard.vue'
  import FormNews from './components/FormNews.vue'
  import FooterInfo from './components/FooterInfo.vue'
</script>

<style lang="scss">
.full-screen-baner {
  position: relative;
}

.header-menu {
  position: absolute;
  z-index: 4;
}
</style>