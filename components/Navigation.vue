<script setup lang="ts">
const linkList = [
  {
    name: 'HOME',
    path: '/',
  },
  {
    name: 'about',
    path: '/about',
  },
  {
    name: 'counter',
    path: '/counter',
  }
]
</script>

<template>
  <ul>
    <li v-for="(item, index) in linkList" :key="index">
      <NuxtLink :to=item.path>{{ item.name }}</NuxtLink>
    </li>
  </ul>
</template>