<script>
import { RouterLink, RouterView } from "vue-router";

export default {
    name: 'Navbar',
    props: ['value']
}
</script>
<template>
    <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/projects">Projects</RouterLink>
        <RouterLink to="/skills">Skills</RouterLink>
    </nav>
    <RouterView />
</template>
<style scoped></style>