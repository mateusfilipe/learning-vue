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
    <p>
      Para acessar meu portfólio
      <a v-bind:href="meu_link" target="_blank">clique aqui</a>.
    </p>
    <Picture />
  </div>
</template>
<script>
import Picture from './Picture.vue'

export default {
  name: "Info",
  components: {
    Picture,
  },
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: true,
      email: "mateus@sample.com",
      meu_link: "https://google.com",
    };
  },
};
</script>