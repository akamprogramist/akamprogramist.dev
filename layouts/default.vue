<template>
  <div class="px-72 dark:bg-slate-800">
    <Navbar />
    <slot />
  </div>
</template>
<script setup>
const colorMode = useColorMode();
</script>
