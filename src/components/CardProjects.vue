<template>
    <div class="flex justify-start gap-5">
        <div class="border-transparent border-[#B0B0B0] bg-[#323443] p-5">
            Test Picture
        </div>
        <div class="gap-5 my-3">
            <p class="text-xs text-[#B0B0B0] font-bold">Web Development</p>
            <h1 class="text-xl font-bold mt-1">{{ element?.title }}</h1>
            <h4 class="text-md text-[#B0B0B0] mt-3">{{ `This is ${element?.title} projects` }}</h4>
        </div>
    </div>
</template>
<script>
export default {
    name: "CardProjects",
    props: ["element"]
}
</script>
<style scoped></style>