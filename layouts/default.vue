<template>
  <div class="bg-gray-100 min-h-screen text-gray-900">
    <Title>{{ title }}</Title>
    <nav class="bg-white shadow text-lg px-6 py-6">
      <div class="container mx-auto flex items-center justify-between px-6">
        <div>
          <NuxtLink to="/">
<!--            <img src="https://nuxtjs.org/img/logo.png" alt="Nuxt.js" class="h-8 w-auto" />-->
            لوگو
          </NuxtLink>
        </div>
        <div>
          <ul class="flex space-x-12 space-x-reverse">
            <li><NuxtLink to="/">خانه</NuxtLink></li>
            <li><NuxtLink to="/about">درباره ی ما</NuxtLink></li>
<!--            <li><NuxtLink to="/contact-us">ارتباط با ما</NuxtLink></li>-->
          </ul>
        </div>
      </div>
    </nav>
    <slot />
  </div>
</template>

<script setup>
  const title = useState('title', ()=> 'وبلاگ Nuxt 3')
</script>

<style>
  body{
    direction: rtl;
  }
  .router-link-active {
    font-weight: bold;
  }
</style>