<script>
export default {
    name: 'Skills'
}
</script>
<template >
    <div class="text-xl font-bold my-5">Skills</div>
    <div class="flex flex-row flex-wrap flex-start mt-5">
        <div class="mr-5" v-for="val in value?.projects">
            <Card :element="val" />
        </div>
    </div>
</template>
<style>
    
</style>