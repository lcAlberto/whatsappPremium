<script setup lang="js">
import Sidebar from "./components/Sidebar.vue";
import Content from "./components/Content.vue";
import DefaultFooter from "./components/Footer.vue";
</script>

<template>
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
