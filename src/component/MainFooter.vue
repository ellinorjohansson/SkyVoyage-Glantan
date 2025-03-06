<script setup lang="ts">
</script>

<template>
  <footer class="footer-content">
    <h2>SkyVoyage</h2>
    <p class="highlight-text">Vi tar dig till nya höjder</p>
    
    <h3>Kontakta oss</h3>
    <p><a class="contact" href="tel:+010010203">Telefon: 01-010203</a></p>
    <p><a class="contact" href="mailto:info@Skyvoyage.se">Mail: info@Skyvoyage.se</a></p>

    <h3>Sociala medier</h3>
   
    <div class="social-media">
      <a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer">
        <i class="fa fa-instagram"></i> 
        <span>Instagram</span>
      </a>
      <a href="https://www.facebook.com" target="_blank" rel="noopener noreferrer">
        <i class="fa fa-facebook"></i> 
        <span>Facebook</span>
      </a>
    </div>

  </footer>
</template>

<style lang="scss" scoped>
footer {
  background-color: $charcoal;
  color: white;
  text-align: center;

  h2 {
    margin: 0;
    font-family: $font-title;
    font-size: $mobile-font-size-title;
    font-style: italic;
    font-weight: 10;
    letter-spacing: 3px;
  }

  .highlight-text {
    font-family: $font-body;
    font-size: $mobile-font-size-heading4-6;
    margin: 0;
}

  h3 {
    font-family: $font-body;
    font-size: $mobile-font-size-heading3;
    margin: 0;
    margin-top: 30px;
  }

  p {
    font-family: $font-body;
    font-size: $mobile-font-size-paragraph;
    margin: 0;
  }


  .contact {
    font-family: $font-body;
    font-size: $mobile-font-size-paragraph;
    color: white;
    text-decoration: none;


    &:hover {
      color: $coral; 
    }
  }

  .footer-content {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .social-media {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
    margin: 20px 20px;
    padding-bottom: 10px;
  }

  a {
    color: $coral;
    font-size: $mobile-font-size-heading4-6;
    font-family: $font-body;
    text-decoration: none;
    flex-direction: row;
    align-items: center;
    transition: all 0.3s;

    span {
      font-size: $mobile-font-size-heading4-6;
      margin-left: 10px;
      color: white;
    }

    i {
      font-size: 2rem;
    }


    &:hover span {
      border-bottom: 2px solid $coral;
      padding-bottom: 3px;
    }
  }
}

  

@media screen and (min-width: 768px) {
}

@media screen and (min-width: 1024px) {
}
</style>
