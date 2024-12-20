<template>
  <div>
    <p>{{ sanoq }}</p>
    <button @click="increment1">
      <img class="images-1" src="../assets/images/image.jpg" alt="" />
    </button>
    <button @click="increment2">
      <img class="images-1" src="../assets/images/image.jpg" alt="" />
    </button>
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
.images-1 {
  width: 400px;
  height: 500px;
  border-radius: 10px;
  margin-top: 10px;
  cursor: pointer;
}
</style>
