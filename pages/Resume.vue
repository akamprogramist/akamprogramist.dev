<template>
  <div class="py-10">
    <div>
      <p class="text-2xl font-semibold my-10">My Resume</p>
    </div>

    <!-- <Tab
      title="Skills"
      class="bg-creamy flex-1 text-primary py-3 px-8 font-semibold rounded-full"
    >
    </Tab> -->
    <TabsWrapper>
      <Tab title="Projects" class="md:py-2 md:px-8"><Projects /></Tab>
      <Tab title="Expirence" class="md:py-2 md:px-8"><Expirence /></Tab>
    </TabsWrapper>
  </div>
</template>
<script setup></script>
