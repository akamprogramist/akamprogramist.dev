<template>
  <div class="py-10">
    <div>
      <p class="text-2xl font-semibold my-10">My Resume</p>
    </div>

    <TabsWrapper>
      <Tab
        title="Skills"
        class="bg-creamy flex-1 text-primary py-3 px-8 font-semibold rounded-full"
      >
      </Tab>
      <Tab title="Projects" class="flex-1 py-2 px-8 font-semibold rounded-full"
        ><Projects
      /></Tab>
      <Tab title="Expirence" class="flex-1 py-2 px-8 font-semibold rounded-full"
        ><Expirence
      /></Tab>
    </TabsWrapper>
  </div>
</template>
<script setup></script>
