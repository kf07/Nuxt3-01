<script setup lang="ts">
const linkList = [
  {
    name: 'HOME',
    pass: '/',
  },
  {
    name: 'about',
    pass: '/about',
  },
  {
    name: 'counter',
    pass: '/counter',
  }
]
</script>

<template>
  <ul>
    <li v-for="(item, index) in linkList" :key="index">
      <NuxtLink :to=item.pass>{{ item.name }}</NuxtLink>
    </li>
  </ul>
</template>