<script setup lang="ts">
// import { ref } from 'vue'

// defineProps<{ msg: string }>()

// const count = ref(0)
</script>

<template>
  <div class="drawer w-min drawer-mobile drop-shadow-xl">
    <input id="my-drawer-2" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content flex flex-col items-center justify-center">
      <!-- Page content here -->
      <label for="my-drawer-2" class="btn btn-primary drawer-button lg:hidden"
        >Open drawer</label
      >
    </div>
    <div class="drawer-side">
      <label for="my-drawer-2" class="drawer-overlay"></label>
      <ul class="menu bg-base-100 w-56 bg-base-100 text-base-content">
        <!-- Sidebar content here -->
        <img src="/static/LOGO VETOR 3C 2.png" class="mx-auto p-5" />
        <li class="border-l-4 border-secondary hover:rounded-r-lg">
            <a>Whatsapp</a>
        </li>
      </ul>
    </div>
    
  </div>
</template>

<style>
</style>