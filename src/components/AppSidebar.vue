<template>
  <div class="sidebar-wrapper">
    <div class="header">
      <div class="title-wrapper">
        <svg
          data-encore-id="icon"
          role="img"
          aria-hidden="true"
          viewBox="0 0 24 24"
          class="library-icon"
        >
          <path
            d="M3 22a1 1 0 0 1-1-1V3a1 1 0 0 1 2 0v18a1 1 0 0 1-1 1zM15.5 2.134A1 1 0 0 0 14 3v18a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V6.464a1 1 0 0 0-.5-.866l-6-3.464zM9 2a1 1 0 0 0-1 1v18a1 1 0 1 0 2 0V3a1 1 0 0 0-1-1z"
          ></path>
        </svg>

        <h2>Your Library</h2>
      </div>

      <button class="add-button">
        <svg
          data-encore-id="icon"
          role="img"
          aria-hidden="true"
          viewBox="0 0 16 16"
          class="plus-icon"
        >
          <path
            d="M15.25 8a.75.75 0 0 1-.75.75H8.75v5.75a.75.75 0 0 1-1.5 0V8.75H1.5a.75.75 0 0 1 0-1.5h5.75V1.5a.75.75 0 0 1 1.5 0v5.75h5.75a.75.75 0 0 1 .75.75z"
          ></path>
        </svg>
      </button>
    </div>

    <div class="cards-wrapper">
      <div class="light-card">
        <h6 class="card-title">Create your first playlist</h6>
        <p class="card-des">It's easy we'll help you</p>
        <button class="card-action primary-button">Create playlist</button>
      </div>
      <div class="light-card">
        <h6 class="card-title">Let's find some podcasts to follow</h6>
        <p class="card-des">We'll keep you updated on new episodes</p>
        <button class="card-action primary-button">Browse podcasts</button>
      </div>
    </div>

    <nav class="sidebar-footer-nav">
      <ul>
        <li>
          <a href="#">Legal</a>
        </li>
        <li>
          <a href="#">Safety & Privacy Center</a>
        </li>
        <li>
          <a href="#">Privacy Policy</a>
        </li>
        <li>
          <a href="#">Cookies</a>
        </li>
        <li>
          <a href="#">About Ads</a>
        </li>
        <li>
          <a href="#">Accessibility</a>
        </li>
      </ul>

      <a href="#" class="cookies-link">Cookies</a>

      <div class="language-toggle">
        <button>
          <svg
            data-encore-id="icon"
            role="img"
            aria-hidden="true"
            viewBox="0 0 16 16"
            class="globe-icon"
          >
            <path
              d="M8.152 16H8a8 8 0 1 1 .152 0zm-.41-14.202c-.226.273-.463.713-.677 1.323-.369 1.055-.626 2.496-.687 4.129h3.547c-.06-1.633-.318-3.074-.687-4.129-.213-.61-.45-1.05-.676-1.323-.194-.235-.326-.285-.385-.296h-.044c-.055.007-.19.052-.391.296zM4.877 7.25c.062-1.771.34-3.386.773-4.624.099-.284.208-.554.329-.806a6.507 6.507 0 0 0-4.436 5.43h3.334zm-3.334 1.5a6.507 6.507 0 0 0 4.436 5.43 7.974 7.974 0 0 1-.33-.806c-.433-1.238-.71-2.853-.772-4.624H1.543zm4.835 0c.061 1.633.318 3.074.687 4.129.214.61.451 1.05.677 1.323.202.244.336.29.391.297l.044-.001c.06-.01.19-.061.385-.296.226-.273.463-.713.676-1.323.37-1.055.626-2.496.687-4.129H6.378zm5.048 0c-.061 1.771-.339 3.386-.772 4.624-.082.235-.171.46-.268.674a6.506 6.506 0 0 0 4.071-5.298h-3.03zm3.031-1.5a6.507 6.507 0 0 0-4.071-5.298c.097.214.186.44.268.674.433 1.238.711 2.853.772 4.624h3.031z"
            ></path>
          </svg>
          English
        </button>
      </div>
    </nav>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped lang="scss">
@use '@/assets/scss/variables' as vars;

.sidebar-wrapper {
  background: vars.color(lesser-dark);
  border-radius: 8px;
  width: clamp(280px, 26%, 420px);
  padding: 8px;
  display: flex;
  flex-direction: column;
}

.header {
  display: flex;
  align-items: center;
  font-weight: bold;
  padding: 4px 8px 8px;
  justify-content: space-between;
  margin-block-end: 32px;

  .library-icon {
    fill: vars.color(light-grey);
  }

  .title-wrapper {
    display: flex;
    align-items: center;
    padding: 4px 8px;
    gap: 12px;
  }

  h2 {
    color: vars.color(light-grey);
    font-size: vars.$text-base-size;
  }

  .add-button {
    display: flex;

    .plus-icon {
      width: 1rem;
      height: 1rem;
    }
  }
}

.cards-wrapper {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.light-card {
  padding: 16px 20px;
  background: vars.color(dark-grey);
  border-radius: 8px;
  margin-block: 8px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;

  .card-title {
    font-size: vars.$text-base-size;
    font-weight: bold;
  }

  .card-des {
    font-size: 14px;
  }

  .card-action {
    margin-top: 20px;
  }
}

.sidebar-footer-nav {
  padding: 12px;
  margin-top: auto;

  ul {
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;

    li a {
      font-size: 11px;
      color: vars.color(light-grey);
    }
  }
}

.cookies-link {
  font-size: 12px;
  font-weight: normal;
  color: vars.color(primary);
}

.language-toggle {
  margin-top: 32px;

  button {
    padding: 8px 15px 8px 32px;
    position: relative;
    border: 1px solid;
    border-radius: 80px;
    color: vars.color(primary);

    .globe-icon {
      height: 16px;
      width: 16px;
      fill: vars.color(primary);
      position: absolute;
      left: 12px;
      top: 50%;
      transform: translateY(-50%);
    }
  }
}
</style>
