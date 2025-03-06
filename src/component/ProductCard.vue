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
    <img :src="image" :alt="title" class="product-image" />
    <h3 class="product-title">{{ title }}</h3>
    <p class="product-paragraph">{{ paragraph }}</p>
    <ReadMoreButton class="product-btn" />
  </div>
</template>

<style lang="scss" scoped>
//mobil
.product-card {
  background-color: $charcoal;
  margin-top: 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 95%;
  min-height: 600px;
  padding-bottom: 15px;
  flex-grow: 1;

  .product-image {
    width: 100%;
    height: 250px;
    object-fit: cover;
    object-position: 0% 70%;
    border-bottom: solid $coral 5px;
    border-radius: 8px 8px 0 0;
  }

  .product-title {
    font-family: $font-body;
    font-size: $mobile-font-size-heading3;
    margin-left: 5%;
    margin-right: 5%;
  }

  .product-paragraph {
    font-family: $font-body;
    font-size: $mobile-font-size-paragraph;
    margin-left: 5%;
    margin-right: 5%;
  }

  .product-btn {
    align-self: flex-end;
    margin-right: 5%;
  }
}
//tablet
@media screen and (min-width: 768px) {
  .product-card {
    width: 45%;
    height: 700px;
    margin: 25px;
    padding-bottom: 20px;

    .product-image {
      height: 300px;
      object-position: center;
      object-fit: cover;
    }

    .product-title {
      font-size: $tablet-font-size-heading3;
    }

    .product-paragraph {
      font-size: $tablet-font-size-paragraph;
    }
  }
}
//desktop
@media screen and (min-width: 1024px) {
}
</style>
