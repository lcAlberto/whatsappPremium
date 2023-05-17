<script setup lang="js">
import Sidebar from "./components/Layout/Sidebar.vue";
import Content from "./components/Content.vue";
import DefaultFooter from "./components/Layout/Footer.vue";
import { onMounted } from 'vue';
onMounted(() => {
  document.title = '3C+ Whatsapp';
});
</script>

<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" />
  <div class="flex bg-base-50 p-0">
    <sidebar />
    <div class="flex flex-col flex-1">
      <main class="h-full mx-auto px-3 w-full">
        <div class="py-4 mx-auto">
          <content />
        </div>
      </main>
      <default-footer />
    </div>
  </div>
</template>

<style scoped>
</style>
