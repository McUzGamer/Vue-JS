<template>
  <div>
    <p>{{ sanoq }}</p>
    <button @click="increment1">Oshirish</button>
    <button @click="increment2">Kamaytirish</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
let sanoq = ref(0);
function increment1() {
  sanoq.value++;
}
function increment2() {
  sanoq.value--;
}
</script>

<style scoped>
button {
  background-color: aqua;
  color: white;
  padding: 11px 33px;
  border: 1px solid transparent;
  border-radius: 8px;
  cursor: pointer;
}
</style>
