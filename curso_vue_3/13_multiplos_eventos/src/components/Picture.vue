<template>
  <img :src="avatar" :alt="descricao" width="80" />
</template>
<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "https://cdn-icons-png.flaticon.com/512/147/147142.png",
      descricao: "Logo Vue",
    };
  },
};
</script>