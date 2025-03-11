<script setup lang="ts">
  import SvgLogoPlane from "./SvgLogoPlane.vue";
</script>

<template>
    <div class="h1-container">
      <h1>SkyVoyage</h1>
      <SvgLogoPlane />
    </div>
</template>

<style lang="scss" scoped>
.h1-container {
  position: absolute;
  top: 20%;
  left: 50%;
  transform: translate(-50%, -49%);
  display: flex;
  align-items: center;
  
  h1 {
    font-size: $mobile-font-size-title;
    color: white;
    font-family: $font-title;
    font-style: italic;
    font-weight: 400;
    letter-spacing: 3px;
  }
}

@media screen and (min-width: 768px) {
  .h1-container {
    left: 2%;
    top: 15%;
    transform: translate(0, -49%);

    h1 {
      font-size: $tablet-font-size-title;
    }
  }
}

@media screen and (min-width: 1024px) {
  .h1-container {
    left: 2%;
    top: 13%;
    transform: translate(0, -49%);

    h1 {
      font-size: $desktop-font-size-title;
    }
  }
}
</style>
