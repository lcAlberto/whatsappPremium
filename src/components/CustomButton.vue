<script>
import axios from "axios"
export default {
  data() {
    return {
      loading: false
    }
  },
  methods: {
    async submit () {
      this.loading = true
      await axios
      .post('https://3cvoice.staging.3cplus.com.br/api/v1/user_data/555?api_token=2v3RzfjOEeBUgSp1PlX0mRHCiSbi19jJispX32oheBsypc5Ra7Bqbech1jTq')
      .then((response) => {
        if (response.status == 200) {
          this.$emit('success')
        }
      }).catch((err) => {
        alert('Erro ao enviar convite')
        console.log(err)
      })
      this.loading = false
    }
  }
};
</script>

<template>
  <button
    class="btn btn-wide btn-primary px-0 min-h-min h-9 w-64 flex"
    :class="{ 'loading': loading }"
    @click="submit"
  >
    <span v-if="loading">Enviando...</span>
    <span v-else>Quero ter acesso antecipado</span>
  </button>
</template>

<style>
</style>
