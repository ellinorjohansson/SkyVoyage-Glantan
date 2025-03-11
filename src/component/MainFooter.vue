<script setup lang="ts"></script>

<template>
  <footer class="footer-content">
    <div class="heading">
      <h2>SkyVoyage</h2>
      <p class="highlight-text">Vi tar dig till nya höjder</p>
    </div>

    <div class="contact-info">
      <h3 class="contact-heading">Kontakta oss</h3>
      <p><a class="contact" href="tel:+010010203">Telefon: 01-010203</a></p>
      <p><a class="contact" href="mailto:info@Skyvoyage.se">Mail: info@Skyvoyage.se</a></p>
    </div>

    <div class="social-media">
      <h3 class="social-heading">Sociala medier</h3>
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
  margin-top: 18px;
  padding-bottom: 40px;

  h2 {
    margin: 0;
    font-family: $font-title;
    font-size: $mobile-font-size-title;
    font-style: italic;
    font-weight: 100;
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

  .contact-info {
    padding-top: 20px;
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
      font-size: $mobile-font-size-paragraph;
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

  footer .heading h2 {
    font-size: $tablet-font-size-heading2;
  }

  footer .heading .highlight-text {
    font-size: $tablet-font-size-heading4-6;
  }

  footer .contact-info h3 {
    font-size: $tablet-font-size-heading3;
  }

  footer .contact-info p {
    font-size: $tablet-font-size-paragraph;
  }

  footer .social-media h3 {
    font-size: $tablet-font-size-heading3;
  }

  footer .social-media span {
    font-size: $tablet-font-size-paragraph;
  }

  .footer-content {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    grid-template-rows: 1fr;
    padding: 20px;
    justify-items: center;
  }

  .contact-info {
    grid-column: 1 / span 2;
    grid-row: 1;
    text-align: left;
    left: 20px;
    margin-top: 25px;

    p {
      margin-top: 5px;
    }
  }

  .heading {
    grid-column: 3 / span 2;
    grid-row: 1;
    text-align: center;
    margin-top: 0;
  }

  .social-media {
    grid-column: 5 / span 2;
    grid-row: 1;
    text-align: right;
  }
  .social-heading {
    margin-top: 25px;
  }
  .social-media a {
    margin-bottom: 0;
  }
}

@media screen and (min-width: 1024px) {
  footer .heading h2 {
    font-size: $desktop-font-size-heading2;
  }

  footer .heading .highlight-text {
    font-size: $desktop-font-size-heading4-6;
  }

  footer .contact-info h3 {
    font-size: $desktop-font-size-heading3;
  }

  footer .contact-info p a {
    font-size: $desktop-font-size-paragraph;
  }

  footer .social-media h3 {
    font-size: $desktop-font-size-heading3;
  }

  footer .social-media span {
    font-size: $desktop-font-size-paragraph;
  }

  .heading {
    margin-top: 15px;
  }
}
</style>
