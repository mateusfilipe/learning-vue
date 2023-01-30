<template>
  <img :src="avatar" :alt="descricao" width="80" />
  <MudarImagem @mudar-imagem="mudarImagem" />
</template>
<script>
import MudarImagem from "./MudarImagem.vue";
export default {
  name: "Picture",
  components: {
    MudarImagem,
  },
  data() {
    return {
      avatar: "https://cdn-icons-png.flaticon.com/512/147/147142.png",
      descricao: "Logo Vue",
      trocado: false,
    };
  },
  methods: {
    mudarImagem() {
      if (!this.trocado) {
        this.avatar = "https://cdn-icons-png.flaticon.com/512/147/147144.png";
      } else {
        this.avatar = "https://cdn-icons-png.flaticon.com/512/147/147142.png";
      }
      this.trocado = !this.trocado;
    },
  },
};
</script>