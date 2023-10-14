<script setup>
import { collection, getDocs } from "firebase/firestore";
import TheWelcome from "../components/TheWelcome.vue";
import { db } from "../firebase";
import { onMounted } from "vue";

onMounted(async () => {
  const querySnapshot = await getDocs(collection(db, "dataList"));
  querySnapshot.forEach((el) => {
    console.log(el.data());
  });
});
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template>
