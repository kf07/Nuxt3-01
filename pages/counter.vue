<script setup lang="ts">
 const { count, doubleCount, increment } = useCounter()
</script>

<template>
  <p>{{count}}</p>
  <p>{{doubleCount}}</p>
  <button @click="increment">increment</button>
</template>
