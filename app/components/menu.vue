<template>
  <nav class="font-mono">
    <ul class="flex flex-col md:flex-row md:space-x-4">
      <li>
        <NuxtLink to="/" class="link">home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about" class="link">about</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/project" class="link">projects </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/blog" class="link">blog </NuxtLink>
      </li>
    </ul>
  </nav>
</template>
<style scoped>
.link {
  @apply p-1 hover:bg-gray-200 hover:dark:bg-gray-800 text-2xl md:text-base;
}
</style>
