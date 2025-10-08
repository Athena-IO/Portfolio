<template>
  <div class="not-prose">
    <section v-if="pending">loading...</section>
    <section v-else-if="error">something went wrong</section>
    <section v-else>
      <ul class="grid grid-cols-1 gap-4">
        <li
          v-for="repository in repos"
          :key="repository.id"
          class="border border-gray-200 dark:border-gray-800 rounded-sm p-4 hover:bg-gray-200 hover:dark:bg-gray-800 font-mono"
        >
          <a :href="repository.html_url" target="_blank">
            <div class="flex items-center justify-between text-sm">
              <div class="font-semibold">{{ repository.name }}</div>
              <div>{{ repository.stargazers_count }}☺</div>
            </div>
            <p>{{ repository.description }}</p>
          </a>
        </li>
      </ul>
    </section>
  </div>
</template>

<script setup>
const { error, pending, data } = await useFetch(
  "https://api.github.com/users/Athena-IO/repos"
);
const repos = computed(() =>
  data.value
    .filter((repo) => repo.description)
    .sort((a, b) => b.stargazers_count - a.stargazers_count)
);
</script>
