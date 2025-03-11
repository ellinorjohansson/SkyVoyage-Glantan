<script lang="ts" setup>
import { ref } from "vue";

const activeLink = ref("");
</script>

<template>
  <nav>
    <ul> 
      <!-- Vi har gjort såhär eftersom det bara är Hem och Boka som ska leda till nya sidor, men vi ville ändå att de andra också skulle bli styleade vid click/hover -->
      <RouterLink class="router-link" to="/"><li :class="{ 'active': activeLink === 'hem' }" @click="activeLink = 'hem'">Hem</li></RouterLink>
      <li :class="{ 'active': activeLink === 'luftballong' }" @click="activeLink = 'luftballong'">Luftballong</li>
      <li :class="{ 'active': activeLink === 'akrobatflyg' }" @click="activeLink = 'akrobatflyg'">Akrobatflyg</li>
      <RouterLink class="router-link" to="/boka"><li :class="{ 'active': activeLink === 'boka' }" @click="activeLink = 'boka'">Boka</li></RouterLink>
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

    .router-link {
      text-decoration: none;
      color: white;
    }

    li {
      cursor: pointer;
      transition: all 0.3s ease;

      &:not(.active):hover {
          text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
        }

      &.active {
          border-bottom: 2px solid $coral;
        }
    }
  }
}

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

@media screen and (min-width: 1024px) {
  nav {
    top: 140px;

    ul {
      font-size: $desktop-font-size-heading2;
      height: 70px;
      justify-content: flex-end;
      padding-right: 60px;

      li {
        margin-left: 30px;
        margin-right: 0;
      }
    }
  }
}
@media screen and (max-width: 767px) {
  nav {
    display: none; 
  }
}
</style>