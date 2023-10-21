<script>
import { RouterLink, RouterView } from "vue-router";

export default {
    name: 'Navbar',
}
</script>
<template>
    <div class="flex justify-between">
        <div class="self-center">
            <h1 class="font-bold text-xl">HARYO PORTOFOLIO</h1>
        </div>
        <div class="flex justify-end m-5">
            <RouterLink class="m-5" to="/">Home</RouterLink>
            <RouterLink class="m-5" to="/skills">Skills</RouterLink>
            <RouterLink class="m-5" to="/projects">Projects</RouterLink>
            <RouterLink class="m-5" to="/testimony">Testimony</RouterLink>
        </div>
        <RouterView />
    </div>
</template>
<style scoped></style>