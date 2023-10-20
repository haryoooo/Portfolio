<script>
import Headers from "../components/Header.vue";
import Projects from "../components/Projects.vue";

export default {
  name: "HomeView",
  components: { Headers, Projects },
  props: ["value", "loading"],
};
</script>

<template>
  <Headers :value="value" :loading="loading" />
  <Projects :value="value" :loading="loading" />
</template>

<style scoped></style>
