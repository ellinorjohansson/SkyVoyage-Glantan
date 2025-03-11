<script setup lang="ts">
import HeaderLogo from "./HeaderLogo.vue";
import NavBar from "./NavBar.vue";
</script>

<template>
  <header>
    <HeaderLogo />
    <img src="/assets/images/Hero_image.jpg" alt="En färgglad luftballong som svävar på en blå himmel" 
      height="1280" width="855" />
    <NavBar />
  </header>
</template>

<style lang="scss" scoped>
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
}

@media screen and (min-width: 768px) {
  header {
    width: 100%;
    height: 445px;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: 0% 0%;
    }
  }
}

@media screen and (min-width: 1024px) {
  header {
    width: 100%;
    height: 690px;
    
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: 0% 30%;
    }
  }
}
</style>