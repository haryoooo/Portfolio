<script>
export default {
  name: "Header",
  props: ["value", "loading"],
};
</script>

<template>
  <div class="border-2 w-32 h-32 rounded-full text-center">Picture</div>
  <div class="text-lg mt-3 ml-2 font-bold">{{ value.name }}</div>
  <div class="text-md ml-2">{{ value.occupation }}</div>
  <div class="text-md my-4 ml-2 font-sm text-[#969696]">
    {{ value.about }}
  </div>
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
