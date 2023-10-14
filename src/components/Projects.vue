<script>
export default {
    name: "Projects",
    props: ["value", "loading"],
};
</script>

<template>
    {{ console.log(value) }}
    <div>My Projects</div>
    <div class="flex flex-start mt-5">
        <div class="w-32 h-32 cursor-pointer">
            <img src="../assets//icons//button-talk.png" alt="talk" />
        </div>
        <div class="w-32 h-32 ml-2 cursor-pointer">
            <img src="../assets//icons//button-linkedin.png" alt="linkedin" />
        </div>
    </div>
</template>

<style scoped></style>
