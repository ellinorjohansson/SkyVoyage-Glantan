<script setup lang="ts">
import { ref } from "vue";

const showCookie = ref(true);

function acceptCookies() {
  showCookie.value = false;
}

function declineCookies() {
  showCookie.value = false;
}
</script>

<template>
  <div class="cookie-wrapper" v-if="showCookie">
    <div class="cookie-container">
      <div class="text-container">
        <h2>Upp i luften!</h2>
        <p>
          Vi använder cookies för att ge dig en smidig och bekväm resa på vår webbplats. Genom att fortsätta surfa godkänner du våra
          små digitala passagerare. Håll i hatten och njut av färden!
        </p>
    </div>
    <div class="button-container">
        <button class="accept-btn" @click="acceptCookies">Acceptera</button>
        <button class="decline-btn" @click="declineCookies">Avböj</button>
    </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.cookie-wrapper {
  position: fixed;
  top: 0;
  width: 100%;
  height: 100vh; 
  background: rgba(98, 98, 98, 0.4); 
  backdrop-filter: blur(5px); 
  z-index: 1000;

  .cookie-container {
    position: fixed;
    top: 20%;
    width: 100%;
    height: 60%;
    background-color: $coral;
    color: black;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    text-align: left;

    .text-container {
      display: flex;
      flex-direction: column;

      h2 {
        font-family: $font-heading2;
        font-size: $mobile-font-size-heading2;
        margin: 0;
        padding-left: 30px;
      }
    
      p {
        font-family: $font-body;
        font-size: $mobile-font-size-paragraph;
        padding-left: 30px;
        padding-right: 30px;
      }
    }
  
    .button-container {
      display: flex;
      flex-direction: column;
      gap: 15px;

      button {
        width: 205px;
        height: 44px;
        box-shadow: 0px 4px 4px 0px #00000040;
        font-family: $font-body;
        font-size: $mobile-font-size-heading3;
        color: white;
        border-radius: 5px;
        border: none;
      }
      
      .accept-btn {
        background-color: $honolulu-blue;
      }
    
      .decline-btn {
        background-color: #595959;
      }
    }
  }
}

@media screen and (min-width: 768px) {
  .cookie-wrapper {
    height: auto;
    background: none; 
    backdrop-filter: none; 

  .cookie-container {
    top: auto;
    bottom: 0;
    width: 100%;
    height: 20%;
    display: flex;
    flex-direction: row;

    .text-container {
      h2 {
        margin-top: 10px;
        font-size: $tablet-font-size-heading2;
      }
    
      p {
        font-size: $tablet-font-size-paragraph;
        margin-bottom: 20px;
      }
    }
  
    .button-container {
      margin-right: 30px;
      
      button{
        width: 160px;
        height: 44px;
        font-size: $tablet-font-size-heading3;
      }
    }
  }
}
}

@media screen and (min-width: 1024px) {
  .cookie-wrapper {
    .cookie-container {
      .text-container {

        h2 {
          font-size:  $desktop-font-size-heading2;
        }
        
        p {
            font-size: $desktop-font-size-paragraph;
        }
      }
    }
  }
}
</style>
