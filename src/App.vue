<script setup lang="ts">
import { RouterView } from "vue-router"
import MainHeader from "./component/MainHeader.vue"
import MainFooter from "./component/MainFooter.vue"
</script>

<template>
  <MainHeader />
  <RouterView />
  <MainFooter />
</template>

<style lang="scss">
body {
  margin: 0;
  box-sizing: border-box;
  background-color: $prussian-blue;
}
</style>
