<template>
  <div
    class="flex backdrop-blur-lg sticky top-0 text-lg justify-between gap-3 items-center py-3"
  >
    <div>
      <NuxtLink to="/" class="">Home</NuxtLink>
    </div>
    <div class="w-64 flex capitalize justify-between">
      <NuxtLink
        to="/about"
        class="rounded-lg my-2 dark:text-secondary hover:opacity-70"
        >About
      </NuxtLink>
      <NuxtLink
        to="/"
        class="rounded-lg my-2 dark:text-secondary hover:opacity-70"
        >Work
      </NuxtLink>
      <NuxtLink
        to="/"
        class="rounded-lg my-2 dark:text-secondary hover:opacity-70"
        >Expirence
      </NuxtLink>
    </div>
    <div>
      <button
        @click="toggleDark"
        v-if="colorMode.value === 'dark'"
        class="flex items-center text-xl p-2.5 rounded-lg bg-creamy hover:opacity-80 text-black"
      >
        <Icon name="material-symbols:sunny-outline-rounded" />
      </button>
      <button
        @click="toggleLight"
        v-else
        class="flex items-center text-xl p-2.5 rounded-lg bg-violet-500 hover:bg-violet-600 text-white"
      >
        <Icon name="material-symbols:dark-mode-outline" />
      </button>
    </div>
  </div>
</template>
<script setup>
const colorMode = useColorMode();
function toggleDark() {
  colorMode.value = "light";
}
function toggleLight() {
  colorMode.value = "dark";
}
</script>
