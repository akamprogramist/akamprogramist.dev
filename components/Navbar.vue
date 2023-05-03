<template>
  <div
    class="flex backdrop-blur-lg sticky top-0 justify-between items-center py-2"
  >
    <NuxtLink to="/" class="">Akam</NuxtLink>
    <div class="flex capitalize items-center gap-3">
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
      <Dropdown>
        <template #MenuItem>
          <div class="capitalize">
            <NuxtLink href="/#about">
              <div class="w-full px-5 py-2 hover:bg-creamy hover:text-black">
                About Me
              </div>
            </NuxtLink>
            <NuxtLink href="/">
              <div class="w-full px-5 py-2 hover:bg-creamy hover:text-black">
                Projects
              </div>
            </NuxtLink>
            <NuxtLink href="/">
              <div class="w-full px-5 py-2 hover:bg-creamy hover:text-black">
                Tech Stack
              </div>
            </NuxtLink>
          </div>
        </template>
      </Dropdown>
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
