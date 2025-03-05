<script setup lang="ts">
import ProductCard from "@/component/ProductCard.vue"
import CardImage from "/assets/images/Card_image.png"
import AerobaticPlane from "/assets/images/aerobatic_plane.jpg"
</script>

<template>
  <main>Hem</main>
  <ProductCard
    :image="CardImage"
    title="Upplev himlen från en ny höjd med luftballong!"
    paragraph="Boka en oförglömlig luftballongfärd med oss och sväv bort 
    över fantastiska landskap. En rofylld och magisk upplevelse som ger 
    perspektiv och minnen för livet. Välkommen att boka din flygning idag!"
  />
  <ProductCard
    :image="AerobaticPlane"
    title="Följ med på en adrenalinfylld resa med akrobatflyg!"
    paragraph="Boka din plats för en adrenalinfylld akrobatflygning och 
    känn vinden i ansiktet när du svävar genom loopar och snabba manövrar. 
    En häftig och vågad upplevelse som får ditt hjärta att slå snabbare. 
    Klar för att ta ut svängarna?"
  />
</template>
