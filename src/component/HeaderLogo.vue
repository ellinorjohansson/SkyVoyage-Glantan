<template>
  <h1>Skyvoyage</h1>
</template>

<style lang="scss" scoped>
h1 {
  position: absolute;
  z-index: 2;
  font-family: $font-title;
  color: white;
  font-size: $mobile-font-size-title;
  font-style: italic;
  font-weight: 400;
  letter-spacing: 3px;
  margin-top: 0;
  left: 25%;
}

@media screen and (min-width: 768px) {
  h1 {
    font-size: $tablet-font-size-title;
    left: 2%;
  }
}

@media screen and (min-width: 1024px) {
  h1 {
    font-size: $desktop-font-size-title;
  }
}
</style>
