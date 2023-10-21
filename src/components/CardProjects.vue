<script>
export default {
  name: "CardProjects",
  props: ["element"],
};
</script>
<template>
  <div class="flex justify-start gap-5 hover:scale-[1.05] mt-3">
    <div
      class="border-transparent w-96 border-[#B0B0B0] bg-[#323443] rounded-lg px-5 py-2"
    >
      <div class="gap-5 my-3">
        <div class="flex flex-row justify-between">
          <div>
            <p class="text-xs text-[#B0B0B0] font-bold">Web Development</p>
          </div>
          <div class="border-transparent">
            <a :href="element?.url" target="_blank">
              <div class="bg-[#3f4152] rounded-lg">
                <img src="../assets/icons/arrow-up.png" alt="arrow-up" />
              </div>
            </a>
          </div>
        </div>
        <h1 class="text-xl font-bold mt-1">{{ element?.title }}</h1>
        <h4 class="text-md text-[#B0B0B0] mt-3">
          {{ `This is ${element?.title} projects` }}
        </h4>
        <div class="flex flex-row justify-start my-3">
          <div
            v-for="(el, index) in element?.technology"
            :key="index"
            class="bg-[#fbfbfb] rounded-lg mr-3"
          >
            <div class="border-transparent">
              <img width="30" :src="el" alt="tech-skill" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped></style>
