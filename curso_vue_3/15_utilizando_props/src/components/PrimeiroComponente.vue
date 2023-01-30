<template>
  <h1>Olá Vue!</h1>
  <Reutilizacao />
  <Reutilizacao />
  <Reutilizacao />
  <Reutilizacao />
  <Reutilizacao />
  <MultiplosEventos />
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue";
import Reutilizacao from "./Reutilizacao.vue";
export default {
  components: {
    MultiplosEventos,
    Reutilizacao,
  },
  name: "PrimeiroComponente",
};
</script>