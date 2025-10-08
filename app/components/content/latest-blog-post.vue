<template>
  <BlogPosts v-slot="{ posts }" :limit="limit">
    <div v-for="post in posts">
      <NuxtLink :to="post._path">{{ post.title }}</NuxtLink>
    </div>
  </BlogPosts>
</template>

<script setup>
const props = defineProps({
  limit: {
    type: Number,
    default: null,
  },
});
</script>
