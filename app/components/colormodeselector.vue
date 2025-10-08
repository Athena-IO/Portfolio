<template>
  <div class="flex space-x-2 items-center">
    <div class="text-gray-500 text-xs" v-if="showNextModelLabel">
      Change to {{ nextMode }}
    </div>

    <button
      @click="colormode"
      @mouseenter="showNextModelLabel = true"
      @mouseleave="showNextModelLabel = false"
      class="hover:bg-gray-200 dark:hover:bg-gray-600 px-2 py-1 text-gray-500 text-4xl md:text-base"
    >
      {{ nextModeIcon }}
    </button>
  </div>
</template>

<script setup>
const colorMode = useColorMode();
const showNextModelLabel = ref(false);

const modes = ["system", "light", "dark"];
const nextModeIcons = {
  system: "🌓",

  light: "🌕",

  dark: "🌑",
};
const nextMode = computed(() => {
  const colorModeIndex = modes.indexOf(colorMode.preference);
  let nextModeIndex = null;
  if (colorModeIndex + 1 == modes.length) {
    nextModeIndex = 0;
  } else {
    nextModeIndex = colorModeIndex + 1;
  }
  return modes[nextModeIndex];
});
const colormode = () => {
  colorMode.preference = nextMode.value;
};

const nextModeIcon = computed(() => nextModeIcons[nextMode.value]);
</script>
