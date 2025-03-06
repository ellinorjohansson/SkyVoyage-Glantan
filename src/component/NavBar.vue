<script lang="ts" setup></script>

<template>
  <nav>
    <ul>
      <li>Hem</li>
      <li>Luftballong</li>
      <li>Akrobatflyg</li>
      <li>Boka</li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  font-family: $font-heading2;
  z-index: 2;
  background-color: rgba(255, 255, 255, 0.38);
  width: 100%;
  position: absolute;
  color: white;

  ul {
    list-style: none;
    display: flex;
    margin: 0;
    align-items: center;
    justify-content: center;
  }
}

//tablet
@media screen and (min-width: 768px) {
  nav {
    top: 120px;
    ul {
      height: 50px;
      font-size: $tablet-font-size-heading2;
      li {
        margin-right: 50px;

      }
    }
  }
}

//desktop
@media screen and (min-width: 1024px) {
  nav {
    height: 70px;
    top: 120px;
    ul {
      font-size: $desktop-font-size-heading2;
      li {
        margin-right: 40px;
      }
    }
  }
}
</style>
