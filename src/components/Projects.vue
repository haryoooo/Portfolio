<script>
import Card from "../components/CardProjects.vue";

export default {
    name: "Projects",
    components: { Card },
    props: ["value", "loading"]
};
</script>

<template>
    {{ console.log("val", value) }}
    <div class="text-xl font-bold">Featured Projects</div>
    <div class="flex flex-start mt-5" v-for="val in value?.projects">
        <Card :element="val" />
    </div>
</template>

<style scoped></style>
