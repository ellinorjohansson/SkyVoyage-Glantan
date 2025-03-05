<script lang="ts" setup>
import ReadMoreButton from "./ReadMoreButton.vue"

defineProps({
  image: String, // Bild-URL
  title: String, // Rubrik
  paragraph: String, // Brödtext
})
</script>

<template>
  <div class="product-card">
    <img :src="image" :alt="title" />
    <h3>{{ title }}</h3>
    <p>{{ paragraph }}</p>
    <ReadMoreButton />
  </div>
</template>

<style lang="scss" scoped>
//mobil
div {
  width: 95%;
  img {
    width: 100%;
  }

  h3 {
    font-family: $font-body;
    font-size: $mobile-font-size-heading3;
  }

  p {
    font-family: $font-body;
    font-size: $mobile-font-size-paragraph;
  }
}
//tablet

//desktop
</style>
