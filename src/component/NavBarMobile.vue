<script lang="ts" setup>
</script>

<template>
  <nav class="bottom-nav">
    <router-link to="/" class="nav-item" aria-label="Gå till startsida">
      <i class="fa-solid fa-house" alt="Husikon för startsida"></i>
    </router-link>

    <div class="nav-item">
      <img src="/assets/images/balloon_icon_orange.png" alt="Luftballong" class="icon" width="400" height="567" />
    </div>

    <div class="nav-item">
      <img src="/assets/images/airplane_icon_orange.png" alt="Flygplan" class="icon" width="646" height="567" />
    </div>

    <router-link to="/boka" class="nav-item" aria-label="Gå till bokningssida">
      <i class="fa-solid fa-calendar-week" alt="Kalenderikon för bokning"></i>
    </router-link>
  </nav>
</template>

<style lang="scss" scoped>
.bottom-nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: $paynes-gray;
  padding: 10px;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  border-top: 2px solid $charcoal; 
  z-index: 100;
  padding: 0;
}

.icon {
  width: 24px; 
  height: 24px;
  object-fit: contain; 
}

.nav-item {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  padding: 8px;
  background-color: $paynes-gray;
}

.nav-item i, .nav-item img {
  color: $coral; 
  font-size: 2.125rem;
  width: 34px; 
  height: 34px;
}

.nav-item:not(:last-child) {
  border-right: 3px solid $charcoal; 
  height: 40px;
}


@media screen and (min-width: 768px) {
  .bottom-nav {
    display: none;
  }

}
</style>