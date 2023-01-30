<template>
  <div>
    <button
      @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro($event)"
    >
      Ativer múltiplos eventos.
    </button>
    <p>{{ multiplos_eventos }}</p>
  </div>
</template>
<script>
export default {
  name: "MultiplosEventos",
  components: {},
  data() {
    return {
      multiplos_eventos: "",
      txt1: "Primeiro evento",
      txt2: "Segundo evento",
    };
  },
  methods: {
    primeiro(txt, e) {
      this.multiplos_eventos = txt;
    },
    segundo(txt, e) {
      setTimeout(() => {
        this.multiplos_eventos = txt;
      }, 500);
    },
    terceiro(txt, e) {
      setTimeout(() => {
        this.multiplos_eventos = "";
      }, 1000);
    },
  },
};
</script>
<style scoped>
div {
  margin: 100px;
}
</style>