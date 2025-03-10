<script setup lang="ts">
  import ProductCard from "@/component/ProductCard.vue"
  import AboutUs from "@/component/AboutUs.vue"
  import CardImage from "/assets/images/Card_image.png"
  import AerobaticPlane from "/assets/images/aerobatic_plane.jpg"
  import ReviewCarousel from "@/component/ReviewCarousel.vue"
</script>

<template>
  <main>
    <AboutUs />
    <div class="product-card-container">
    <ProductCard
      :image="CardImage"
      alt="En färgglad luftballong som svävar på en blå himmel"
      title="Upplev himlen från en ny höjd med luftballong!"
      paragraph="Boka en oförglömlig luftballongfärd med oss och sväv bort 
      över fantastiska landskap. En rofylld och magisk upplevelse som ger 
      perspektiv och minnen för livet. Välkommen att boka din flygning idag!"
    />
    <ProductCard
      :image="AerobaticPlane"
      alt="Ett akrobatflygplan i luften som gör en manöver"
      title="Följ med på en adrenalinfylld resa med akrobatflyg!"
      paragraph="Boka din plats för en adrenalinfylld akrobatflygning och 
      känn vinden i ansiktet när du svävar genom loopar och snabba manövrar. 
      En häftig och vågad upplevelse som får ditt hjärta att slå snabbare. 
      Klar för att ta ut svängarna?"
    />
    </div>
    <ReviewCarousel />
  </main>
</template>

<style lang="scss" scoped>
.product-card-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;
  background-color: $prussian-blue;
}

@media screen and (min-width: 768px) {
  .product-card-container {
    flex-direction: row;
    justify-content: center;
  }
}

@media screen and (min-width: 1024px) {
  .product-card-container {
    height: 550px;
    padding: 45px;
  }
}
</style>
