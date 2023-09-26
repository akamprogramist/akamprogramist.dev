<template>
  <Menu as="div" class="relative">
    <div class="group">
      <MenuButton
        class="flex items-center text-xl p-2.5 border border-zinc-700 dark:border-zinc-400 rounded-lg hover:opacity-60 duration-150"
      >
        <Icon name="ic:round-menu" />
      </MenuButton>
    </div>

    <transition
      enter-active-class="transition duration-100 ease-out"
      enter-from-class="transform scale-95 opacity-0"
      enter-to-class="transform scale-100 opacity-100"
      leave-active-class="transition duration-75 ease-in"
      leave-from-class="transform scale-100 opacity-100"
      leave-to-class="transform scale-95 opacity-0"
    >
      <MenuItems
        class="absolute mt-1 w-52 right-0 bg-[#F5F0E8] dark:bg-zinc-800 rounded shadow"
      >
        <div class="py-2">
          <slot name="MenuItem">
            <MenuItem>
              <slot />
            </MenuItem>
          </slot>
        </div>
      </MenuItems>
    </transition>
  </Menu>
</template>

<script setup>
import { Menu, MenuButton, MenuItems, MenuItem } from "@headlessui/vue";
const props = defineProps({
  title: String,
});
</script>
