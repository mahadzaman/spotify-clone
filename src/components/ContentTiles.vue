<template>
  <section class="content-section-wrapper">
    <div class="content-header">
      <h5 class="section-title">{{ title }}</h5>
      <a href="#" class="showall-button">Show all</a>
    </div>

    <div class="tiles-wrapper">
      <slot name="tilesWrapper"></slot>
    </div>
  </section>
</template>

<script setup lang="ts">
interface Props {
  title: string
  showAllLink?: string
}

defineProps<Props>()
</script>

<style scoped lang="scss">
.content-section-wrapper {
  margin-block-end: 24px;
}
.content-header {
  display: flex;
  justify-content: space-between;
  margin-bottom: 16px;
  padding-top: 16px;

  .section-title {
    font-size: 24px;
    font-weight: bold;
  }

  .showall-button {
    font-size: 14px;

    &:hover {
      text-decoration: underline;
    }
  }
}

.tiles-wrapper {
  display: flex;
  margin-inline: -12px;
}
</style>
