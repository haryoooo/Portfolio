<script>
export default {
  name: "Header",
  props: ["value", "loading"],
};
</script>

<template>
  <div class="text-center">
    <div class="flex justify-center mb-5">
      <div class="border-2 w-48 h-48 rounded-full">
        <img class="rounded-full" src="../assets/images/self-pic.png" alt="self-pic" />
      </div>
    </div>
    <div class="text-lg my-2 ml-2 font-bold">{{ value?.name }}</div>
    <div class="text-md ml-2">{{ value?.occupation }}</div>
    <div class="text-md my-4 ml-2 font-sm text-[#969696]">
      {{ value?.about }}
    </div>
    <div class="flex flex-start justify-center text-center mt-5">
      <div class="w-32 h-32 cursor-pointer mr-5">
        <img src="../assets//icons//button-talk.png" alt="talk" />
      </div>
      <div class="w-32 h-32 ml-2 cursor-pointer">
        <img src="../assets//icons//button-linkedin.png" alt="linkedin" />
      </div>
    </div>
  </div>
</template>

<style scoped></style>
