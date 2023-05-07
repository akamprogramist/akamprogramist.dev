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
      <p class="dark:text-creamy text-bluesh">Hi, My Name is</p>
      <p class="text-6xl font-bold tracking-wide">
        Akam
        <span class="kamal">Kamal</span>
      </p>
    </div>
    <div>
      <p class="text-center my-5">
        I’m a software engineer specializing in building (and occasionally
        designing) exceptional digital experiences. Currently, I’m focused on
        building accessible, human-centered products at Upstatement.
      </p>
    </div>
    <div class="flex justify-center gap-4 my-7">
      <button
        class="flex bg-bluesh dark:bg-creamy text-black font-bold py-3 px-8 items-center border dark:hover:bg-opacity-0 dark:border-creamy dark:hover:text-creamy border-bluesh rounded duration-300"
      >
        Get in Touche
      </button>
      <button
        class="flex text-creamy font-bold py-3 px-8 items-center border dark:hover:bg-creamy dark:border-creamy dark:hover:text-black border-bluesh rounded duration-300"
      >
        View CV
      </button>
    </div>
    <div class="flex gap-4 my-5 text-3xl justify-center">
      <Icon
        name="mdi:github"
        class="hover:-mt-2 grid rounded-full duration-300"
      />
      <Icon
        name="mdi:facebook"
        class="hover:-mt-2 grid rounded-full duration-300"
      />
      <Icon
        name="mdi:instagram"
        class="hover:-mt-2 grid rounded-full duration-300"
      />
    </div>
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
