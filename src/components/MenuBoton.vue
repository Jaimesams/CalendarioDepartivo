<template>
  <button @click="AltMenu">
    <img src="@/assets/menudesplegable.png" alt="Menu Desplegable" />
  </button>
</template>

<script>
export default {
  methods: {
    AltMenu() {
      this.$emit("Alt-Menu");
    },
  },
};
</script>

<style scoped>
button {
  border-radius: 15px;
  background: rgb(6, 82, 82);
  border: none;
  border-top-right-radius: 5em 50%;
  cursor: pointer;
}
</style>
