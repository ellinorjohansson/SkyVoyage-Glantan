<script setup lang="ts">
import { RouterView } from "vue-router"
import MainHeader from "./component/MainHeader.vue"
import MainFooter from "./component/MainFooter.vue"
import NavBarMobile from "./component/NavBarMobile.vue";
</script>

<template>
  <MainHeader />
  <RouterView />
  <MainFooter />
  <NavBarMobile />
</template>

<style lang="scss">
body {
  margin: 0;
  box-sizing: border-box;
  background-color: $prussian-blue;
}
</style>
