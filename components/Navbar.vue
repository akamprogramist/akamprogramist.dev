<template>
  <div
    class="flex backdrop-blur sticky top-0 text-lg justify-between gap-3 items-center p-2"
  >
    <div>
      <NuxtLink to="/" class="flex items-center gap-1"
        ><Icon name="mdi:home" />Home</NuxtLink
      >
    </div>
    <div class="w-80 flex capitalize justify-between">
      <NuxtLink
        to="/"
        class="px-5 py-2 rounded-lg hover:bg-gray-100 dark:hover:bg-grayish"
        >About</NuxtLink
      >
      <NuxtLink
        to="/"
        class="px-5 py-2 rounded-lg hover:bg-gray-100 dark:hover:bg-grayish"
        >projects</NuxtLink
      >
      <NuxtLink
        to="/"
        class="px-5 py-2 rounded-lg border hover:bg-gray-100 dark:hover:bg-grayish"
        >resume</NuxtLink
      >
    </div>

    <select v-model="$colorMode.preference">
      <option value="dark">dark</option>
      <option value="light">light</option>
    </select>
  </div>
</template>
<script setup>
const colorMode = useColorMode();
</script>
