<template>
  <div>
    <Title>صفحه اصلی</Title>
    <nav>
      <ul>
        <li><NuxtLink to="/">خانه</NuxtLink></li>
        <li><NuxtLink to="/about">درباره ی ما</NuxtLink></li>
        <li><NuxtLink to="/posts">پست ها</NuxtLink></li>
      </ul>
    </nav>
    <slot />
  </div>
</template>