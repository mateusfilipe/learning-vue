<template>
  <PrimeiroComponente />
  <Header />
  <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
  <LifeCycle />
  <Pessoa />
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Header,
  },
};
</script>
<style>
body {
  background-color: #333;
  color: #fff;
}
a {
  color: red;
}
.teste {
  background: #000;
}
</style>