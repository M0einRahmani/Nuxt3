<template>
  <div class="container mx-auto w-1/2 py-8">
    <Title>{{ $route.params.id }} | {{ title }}</Title>
    <h3 class="text-3xl font-bold">
      <NuxtLink :to="'/posts/1'">title of post</NuxtLink>
    </h3>
    <div class="post-meta text-gray-700 flex items-center space-x-2 space-x-reverse">
      <div>29 مرداد 1401</div>
      <div>&middot;</div>
      <div>معین رحمانی</div>
    </div>
    <div class="post-content mt-4">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. At esse fugit illo iure magni maxime minus nesciunt pariatur perferendis ut. Blanditiis delectus deleniti dolorem, dolores ea eveniet ex harum in molestiae odit, quaerat quibusdam recusandae rem suscipit tempore temporibus voluptates?
    </div>
  </div>
</template>

<script setup>
const title = useState('title', ()=> 'وبلاگ Nuxt 3')
</script>