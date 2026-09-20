<script setup lang="ts">
  import { ref, computed } from 'vue';

  const count = ref<number>(0)
  const doubleCount = computed(() => count.value * 2) 

  const increment = () => { count.value++ }
  const decrement = () => { count.value-- }
</script>

<template>
  <h1>Counter</h1>
  <p>Count: {{ count }}</p>
  <p>Double Count: {{ doubleCount }}</p>
  <button @click="increment">Increment</button>
  <button @click="decrement">Decrement</button>
</template>


