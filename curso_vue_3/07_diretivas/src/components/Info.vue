<template>
  <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Não estou trabalhando no momento.</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
      <li>Vue.js</li>
      <li>Python</li>
      <li>Php</li>
    </ul>
    <p v-show="mostrar_email">Manda uma mensagem para: {{ email }}</p>
  </div>
</template>
<script>
export default {
  name: "Info",
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: true,
      email: "mateus@sample.com",
    };
  },
};
</script>