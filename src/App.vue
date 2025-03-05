<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router"
import MainHeader from "./component/MainHeader.vue"
import NavBar from "./component/NavBar.vue"
</script>

<template>
  <MainHeader />
  <NavBar />
  <div class="wrapper">
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </div>

  <RouterView />
</template>

<style lang="scss">
body {
  margin: 0;
  box-sizing: border-box;
}
</style>
