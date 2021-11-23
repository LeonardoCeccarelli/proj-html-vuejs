<template>
  <div>
    <div class="subscribe_container">
      <div class="icon_sx_container">
        <i class="fa fa-circle-o" aria-hidden="true"></i>
      </div>
      <div class="subscribe_content_input">
        <h2 class="title_subscribe m_bottom">
          Subscribe <span class="mark_title">Newseletters</span>
        </h2>
        <p class="subtitle_subscribe">
          Enter your email address to register to our newseletter subscription
          delivered on a regular basis!
        </p>
        <div class="form">
          <input type="text" placeholder="Enter your email" />
          <button type="button" class="btun btun_primary">Subscribe</button>
        </div>
      </div>
      <div class="icon_dx_container">
        <img
          class="circle_image"
          src="@/assets/maxcoach-shape-09.png"
          alt="circle image"
        />
        <img
          class="dot_image"
          src="@/assets/maxcoach-shape-02.png"
          alt="dot image"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubscribeMain",
};
</script>

<style>
</style>