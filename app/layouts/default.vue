<template>
  <div class="container mx-auto max-w-2xl">
    <header class="flex justify-between items-start md:items-center mt-5">
      <div class="flex justify-between md:space-x-12">
        <div class="hidden md:block">
          <NuxtLink
            to="/"
            class="text-xl font-semibold p-2 hover:bg-gray-200 hover:dark:bg-gray-800"
            >Athena-IO</NuxtLink
          >
        </div>
        <Menu />
      </div>
      <ClientOnly>
        <Colormodeselector />
      </ClientOnly>
    </header>
    <main class="p-2 mb-10">
      <slot />
    </main>
  </div>
</template>
<script setup></script>

<style>
body {
  font-family: "Roboto";
}
body {
  @apply bg-white dark:bg-gray-900 text-gray-700 dark:text-gray-300;
}
</style>
