<script setup lang="ts">

</script>

<template>
  <div class="drawer w-min drawer-mobile drop-shadow-xl">
    <input id="my-drawer-2" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content flex flex-col items-center justify-center">
      <label for="my-drawer-2" class="btn btn-primary drawer-button lg:hidden"
        >Open drawer</label
      >
    </div>
    <div class="drawer-side">
      <label for="my-drawer-2" class="drawer-overlay"></label>
      <ul class="menu bg-base-100 w-56 bg-base-100 h-full text-base-content">
        <img src="../../assets/img/LOGO VETOR 3C 2.png" class="mx-auto p-5" />
        <li class="border-l-4 border-secondary hover:rounded-r-lg flex flex-row">
          <a><i class="fa fa-whatsapp ml-2"></i>Whatsapp</a>
        </li>
      </ul>
    </div>
    
  </div>
</template>

<style>
</style>