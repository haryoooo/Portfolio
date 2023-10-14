<script>
import Header from "../components/Header.vue";

export default {
  name: "HomeView",
  components: { Header },
  props: ["value", "loading"],
};
</script>

<template>
  <Header :value="value" :loading="loading" />
</template>

<style scoped></style>
