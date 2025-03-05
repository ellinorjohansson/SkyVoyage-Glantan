<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import MainHeader from "./component/MainHeader.vue";


</script>

<template>
  <MainHeader />

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
  }
</style>