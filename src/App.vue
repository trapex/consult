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




  <!--<header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>-->
</template>

<style scoped>

</style>
