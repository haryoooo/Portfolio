<script>
import Card from "../components/CardProjects.vue";

export default {
    name: "Projects",
    components: { Card },
    props: ["value", "loading"]
};
</script>

<template>
    <div class="my-10">
        <div class="text-xl font-bold my-5">Featured Projects</div>
        <div class="flex flex-row flex-wrap flex-start mt-5">
            <div class="mr-5" v-for="val in value?.projects">
                <Card :element="val" />
            </div>
        </div>
    </div>
</template>

<style scoped></style>
