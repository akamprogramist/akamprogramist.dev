<template>
  <div class="grid grid-cols-1 py-24">
    <!-- <div>
      <img
        src="../assets/images/akamprogramist.jpg"
        class="w-32 h-32 rounded-full"
        alt=""
      />
    </div> -->

    <div class="my-5 space-y-3 text-center capitalize">
      <p class="dark:text-creamy text-lg text-bluesh">Hi, My Name is</p>
      <p class="text-8xl font-bold tracking-wide">
        Akam
        <span class="kamal">Kamal</span>
      </p>
    </div>
    <div>
      <p class="text-4xl font-bold tracking-wide leading-snug text-center my-5">
        Building digital products, brands,<br />
        and experience.
      </p>
    </div>
    <div class="flex justify-center gap-4 my-7">
      <button
        class="flex bg-bluesh dark:bg-creamy text-black font-bold py-4 px-14 items-center border dark:hover:bg-opacity-0 dark:border-creamy dark:hover:text-creamy border-bluesh rounded duration-300"
      >
        Get in Touche
      </button>
      <button
        class="flex text-creamy font-bold py-4 px-14 items-center border dark:hover:bg-creamy dark:border-creamy dark:hover:text-black border-bluesh rounded duration-300"
      >
        About Me
      </button>
    </div>
    <!-- <div class="flex gap-4 my-5 justify-center">
      <Icon name="mdi:github" class="text-3xl" />
      <Icon name="mdi:facebook" class="text-3xl" />
      <Icon name="mdi:instagram" class="text-3xl" />
    </div> -->
  </div>
</template>
<script setup></script>

<style scoped>
.kamal {
  color: #202023;
  -webkit-text-fill-color: transparent; /* Will override color (regardless of order) */
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: #202023;
}
.dark .kamal {
  color: #ededee;
  -webkit-text-fill-color: transparent; /* Will override color (regardless of order) */
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: #ededee;
}
</style>
