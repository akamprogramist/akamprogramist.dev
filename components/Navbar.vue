<template>
  <div
    class="flex backdrop-blur-lg sticky top-0 justify-between items-center py-2"
  >
    <NuxtLink to="/" class="">Akam</NuxtLink>
    <div class="flex capitalize items-center gap-3">
      <div>
        <button
          @click="toggleLight"
          v-if="colorMode.value === 'light'"
          class="flex items-center text-xl p-2.5 rounded-lg bg-bluesh hover:bg-blueshy text-white"
        >
          <Icon name="material-symbols:dark-mode-outline" />
        </button>
        <button
          @click="toggleDark"
          v-else
          class="flex items-center text-xl p-2.5 rounded-lg bg-creamy hover:opacity-80 text-black"
        >
          <Icon name="material-symbols:sunny-outline-rounded" />
        </button>
      </div>
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
