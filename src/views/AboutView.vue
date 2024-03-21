<script setup lang="ts">
import TheCounter from '@/components/TheCounter.vue'
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <TheCounter />
  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  h1 {
    font-weight: 500;
    font-size: 2.6rem;
  }
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
