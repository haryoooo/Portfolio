<script>
import Headers from "../components/Header.vue";
import Projects from "../components/Projects.vue";
import Skills from "../components/Skills.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "HomeView",
  components: { Headers, Projects, Footer, Skills },
  props: ["value", "loading"],
};
</script>

<template>
  <Headers :value="value" :loading="loading" />
  <Projects :value="value" :loading="loading" />
  <Skills :value="value" :loading="loading" />
  <Footer />
</template>

<style scoped></style>
