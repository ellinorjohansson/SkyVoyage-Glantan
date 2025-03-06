<script setup lang="ts">
import HeaderLogo from "./HeaderLogo.vue"
import NavBar from "./NavBar.vue"
</script>

<template>
  <header>
    <HeaderLogo />
    <img src="/assets/images/Hero_image.jpg" alt="" height="1280" width="855" />
    <NavBar />
    <div class="test">test</div>
  </header>
</template>

<style lang="scss" scoped>
// mobile
header {
  position: relative;
  width: 100%;
  height: 145px;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 0 35%;
  }
  .test {
    background-color: red;
  }
}

// tablet
@media screen and (min-width: 768px) {
  header {
    img {
      width: 100%;
      height: 445px;
      object-fit: cover;
      object-position: 0% 0%;
    }
    .test {
      background-color: aqua;
    }
  }
}

//desktop
@media screen and (min-width: 1024px) {
  header {
    img {
      width: 100%;
      height: 690px;
      object-fit: cover;
      object-position: 0% 30%;
    }
    .test {
      background-color: brown;
    }
  }
}
</style>
