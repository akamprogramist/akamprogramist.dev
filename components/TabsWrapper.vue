<template>
  <div class="tabs">
    <ul
      class="tabs__header grid rounded-3xl md:py-0 grid-cols-2 md:flex md:rounded-full md:text-lg items-center text-center bg-primary border border-stone-700"
    >
      <li
        v-for="title in tabTitles"
        :key="title"
        @click="selectedTitle = title"
        class="flex-1 py-2 px-8 font-semibold rounded-full cursor-pointer"
        :class="title == selectedTitle ? 'bg-creamy text-black' : ''"
      >
        {{ title }}
      </li>
    </ul>
    <slot />
  </div>
</template>
<script setup>
import { ref, provide, useSlots } from "vue";
const tabTitles = ref();
tabTitles.value = useSlots()
  .default()
  .map((tab) => tab.props.title);
const selectedTitle = ref(tabTitles.value[0]);
provide("selectedTitle", selectedTitle);
</script>
