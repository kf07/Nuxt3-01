<script setup lang="ts">
  const count = ref(1)
  const double = computed(() => count.value * 2)
  const increment = () => {
    count.value++;
  }
</script>

<template>
  <p>{{count}}</p>
  <p>{{double}}</p>
  <button @click="increment">increment</button>
</template>
