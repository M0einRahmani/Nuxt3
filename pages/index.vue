<template>
  <div class="container mx-auto w-1/2 py-8 divide-y space-y-8 divide-gray-300">
    <postItem v-for="post in posts" :key="post.id" :post="post"/>
  </div>
</template>

<script setup>
  const { data :posts } = await useFetch('http://127.0.0.1:8000/api/posts')
</script>