<script setup lang="ts">
import { RouterView } from 'vue-router'
import PublicHeader from './components/layouts/PublicHeader.vue'
import SignupFooter from './components/layouts/SignupFooter.vue'
</script>

<template>
  <main>
    <public-header />
    <RouterView />
    <signup-footer />
  </main>
</template>

<style scoped lang="scss">
main {
  display: flex;
  flex-direction: column;
  min-height: 100dvh;
}
</style>
