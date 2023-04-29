<template>
  <div class="dark:bg-slate-900">
    <h1>Color mode: {{ $colorMode.value }}</h1>
    <select v-model="$colorMode.preference">

    </select>
  </div>
</template>
