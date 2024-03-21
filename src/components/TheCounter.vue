<script setup lang="ts">
import { useCounterStore } from '@/stores/counter'

const counter = useCounterStore()
</script>

<template>
  <section class="count-section">
    <h2>Counter</h2>
    <button @click="counter.increment()">Increment</button>
    <button @click="counter.clear()">Clear</button>
    <div>Counter: {{ counter.count }}</div>
    <div>Counter x2: {{ counter.doubleCount }}</div>
  </section>
</template>

<style scoped>
.count-section {
  font-size: 1.25rem;
}
.h2 {
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
}
button {
  font-size: 1.25rem;
  padding: 0.875rem 1.5rem;
}
</style>
