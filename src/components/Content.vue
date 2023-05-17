<script setup lang="ts">
import Navbar from "./Layout/Navbar.vue";
import CustomButton from "./CustomButton.vue";
import { ref } from 'vue'


let success = ref(false)
let title = ref('Quer ter acesso antecipado ao Whatsapp da 3C Plus?')
let subTitle = ref('O Whatsapp da 3C Plus está chegando e você pode entrar para a lista de primeiros usuários')

function toggleMessage() {
  title.value = 'Você já está na lista VIP do Whatsapp da 3C Plus'
  subTitle.value = 'Nosso time entrará em contato em breve para mais informações'
  success.value = true;
}
</script>

<template>
  <navbar :registered="success" @hidde="toggleMessage" />
  <div class="p-0 m-0">
    <div
      class="card grid md:grid-cols-2 items-center justify-items-center gap-3 px-5"
    >
      <div class="prose px-5">
        <img
          v-if="success"
          src="../assets/img/check-circle.png" class="my-0" />
        <img
          v-else
          src="../assets/img/whatsapp.png" class="my-0" />
        <h2 class="text-h2 my-3 font-cerebri">
          {{ title }}
        </h2>
        <p>
          {{ subTitle }}
        </p>
        <custom-button v-if="!success" @success="toggleMessage" />
      </div>
      <div>
        <img src="../assets/img/Home - Whatsapp.png" class="w-96" />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
