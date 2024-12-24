<template>
  <section class="signup-footer-section">
    <div class="signup-footer-wrapper">
      <div class="content-wrapper">
        <p class="footer-title">Preview of Spotify</p>
        <p>
          Sign up to get unlimited songs and podcasts with ocassional ads. No credit card needed.
        </p>
      </div>
      <a href="" class="primary-button">Sign up free</a>
    </div>
  </section>
</template>

<script setup lang="ts"></script>

<style lang="scss">
.signup-footer-section {
  padding-inline: 8px;
  padding-block-end: 8px;
}
.signup-footer-wrapper {
  background: linear-gradient(90deg, #af2896, #509bf5);
  display: flex;
  justify-content: space-between;
  padding: 13px 24px 9px 15px;

  .content-wrapper {
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  .footer-title {
    font-weight: bold;
    font-size: 14px;
  }
}
</style>
