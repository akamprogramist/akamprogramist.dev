<template>
  <div class="py-3 md:flex justify-between items-center">
    <div class="flex gap-2 justify-center">
      <p>&copy;</p>
      <p>2023</p>
      <NuxtLink
        to="/"
        class="tracking-wide text-bluesh dark:text-creamy hover:opacity-80 duration-150"
        >Akam Kamal</NuxtLink
      >
    </div>
    <div
      class="flex capitalize py-3 items-center justify-center text-2xl gap-10"
    >
      <icon
        name="ri:facebook-fill"
        class="hover:text-bluesh dark:hover:text-creamy duration-150"
      ></icon>
      <icon
        name="ri:linkedin-fill"
        class="hover:text-bluesh dark:hover:text-creamy duration-150"
      ></icon>
      <icon
        name="ri:twitter-fill"
        class="hover:text-bluesh dark:hover:text-creamy duration-150"
      ></icon>
      <icon
        name="ri:instagram-fill"
        class="hover:text-bluesh dark:hover:text-creamy duration-150"
      ></icon>
    </div>
  </div>
</template>
