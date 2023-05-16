<script setup lang="ts">
import Navbar from "./Navbar.vue";
import CustomButton from "./CustomButton.vue";
// import DefaultFooter from "./Footer.vue";
// import Content from "./components/Content.vue";
// import { ref } from "vue";

// defineProps<{ msg: string }>();

// const count = ref(0);
</script>

<template>
  <navbar />
  <div class="p-0 m-0">
    <div class="card grid grid-cols-2 items-center justify-items-center gap-3 px-5">
      <div class="prose px-5">
        <h2 class="text-h2">
          Quer ter acesso antecipado ao Whatsapp da 3C Plus?
        </h2>
        <p>
          O Whatsapp da 3C Plus está chegando e você pode entrar para a lista de
          primeiros usuários
        </p>
        <custom-button />
      </div>
      <div>
        <img src="../../static/Home - Whatsapp.png" class="w-96" />
      </div>
    </div>
  </div>
  <!-- <default-footer /> -->
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
