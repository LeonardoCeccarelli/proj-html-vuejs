<template>
  <div class="hero_section_container">
    <!-- Barra laterale dx -->
    <div class="overlay_icon">
      <i class="fa fa-bar-chart"></i>
      <i class="fa fa-sign-in"></i>
      <i class="fa fa-book"></i>
      <i class="fa fa-shopping-cart"></i>
    </div>
    <div class="hero_section_content">
      <!-- Sezione testo -->
      <div class="text_container">
        <div>
          <p class="m_bottom head_title">New Challenge, New Skills</p>
          <!-- Titolo -->
          <h1 class="m_bottom">Build your own life coaching buisness</h1>
          <p class="m_bottom sub_title">
            Whole-Life Buisness Coaching for committed enterpreneurs
          </p>
          <button class="btun btun_primary" type="button">
            Get started today
          </button>
        </div>
      </div>
      <!-- Sezione immagini -->
      <div class="image_container">
        <img
          src="@/assets/home-business-hero-global-image.png"
          alt="global image"
          class="background_global"
        />
        <img src="@/assets/home-business-hero-avatar.png" alt="avatar image" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainHero",
};
</script>

<style>
</style>