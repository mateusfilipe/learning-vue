<template>
  <img :src="avatar" :alt="descricao" width="80" />
  <Reutilizacao />
</template>
<script>
import Reutilizacao from "./Reutilizacao.vue";

export default {
  name: "Picture",
  components: {
    Reutilizacao,
  },
  data() {
    return {
      avatar: "https://cdn-icons-png.flaticon.com/512/147/147142.png",
      descricao: "Logo Vue",
    };
  },
};
</script>