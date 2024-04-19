<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/layout/Header.vue'
import Content from './components/layout/Content.vue'
import Footer from './components/layout/Footer.vue'
</script>

<template>
  <Header/>

  <Content>
    <RouterView />
  </Content>

  <Footer/>

</template>

<style scoped>

</style>
