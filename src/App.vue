<script setup lang="ts">

import { RouterView } from "vue-router";
import MainHeader from "./component/MainHeader.vue";
import MainFooter from "./component/MainFooter.vue";
import CookieNotification from "./component/CookieNotification.vue";
import NavBarMobile from "./component/NavBarMobile.vue";

</script>

<template>
  <MainHeader />
  <RouterView />
  <MainFooter />
  <NavBarMobile />
  <CookieNotification />
</template>

<style lang="scss">
body {
  margin: 0;
  box-sizing: border-box;
  background-color: $prussian-blue;
  overflow-x: hidden;
}
</style>
