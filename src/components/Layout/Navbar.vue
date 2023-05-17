<script setup lang="ts">
import CustomButton from "../CustomButton.vue";
import { ref } from 'vue'

let success = ref(false)
const emit = defineEmits(['hidde'])

const props = defineProps({
  registered: { type: String, required: true },
})

function toggleMessage() {
  success.value = false
  emit('hidde')
}
</script>

<template>
  <div class="navbar bg-base-100">
    <div class="flex justify-between w-full">
      <div class="prose my-10 px-8">
        <h1 class="font-RG">Whatsapp 3C +</h1>
      </div>
      <custom-button class="hidden md:block" v-if="!success && !registered" @success="toggleMessage" />
    </div>
  </div>
</template>

<style>

</style>
