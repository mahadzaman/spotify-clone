<template>
  <div class="tile-wrapper">
    <img
      :src="imgSrc"
      alt="Album Image"
      :class="[tileType === 'flat' ? 'flat-image' : 'circled-image']"
    />
    <p class="tile-title">{{ title }}</p>
    <p class="tile-subtitle">{{ subTitle }}</p>
  </div>
</template>

<script setup lang="ts">
interface Props {
  imgSrc: string
  tileType: 'circle' | 'flat'
  title: string
  subTitle: string
}

withDefaults(defineProps<Props>(), {
  tileType: 'flat',
})
</script>

<style scoped lang="scss">
@use '@/assets/scss/variables' as vars;

.tile-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex: 0 0 calc(100% / 7);
  max-width: calc(100% / 7);
  padding-inline: 12px;

  img {
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.5);
    max-width: 100%;

    &.flat-image {
      border-radius: 6px;
    }

    &.circled-image {
      border-radius: 50%;
    }
  }

  .tile-title {
    margin-top: 6px;
  }

  .tile-subtitle {
    font-size: 14px;
    color: vars.color(light-grey);
    margin-top: 6px;
  }
}
</style>
