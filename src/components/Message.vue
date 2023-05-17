<template>
  
</template>

<script>
import CustomButton from "./CustomButton.vue";
export default {
    props: {
        success: { type: Boolean, required: false },
        mainMessage: { type: String, required: true },
        comment: { type: String, required: true },
        fail: { type: Boolean, required: false },
    }
};
</script>

<style>
</style>