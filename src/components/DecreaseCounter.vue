<script setup>
import { ref } from 'vue'

const decrease = ref(0)

const decreaseCounter = () => {
  decrease.value--
}
</script>

<template>
  <div class="counter">
    <h2>Decrease Counter</h2>
    <button @click="decreaseCounter">-</button>
   
    <span>{{ decrease }}</span>
  </div>
</template>

<style scoped>
.counter {
  text-align: center;
  margin: 20px;
}

button {
  font-size: 24px;
  padding: 10px 20px;
  cursor: pointer;
  background-color: #081308;
  color: white;
  border: none;
  border-radius: 5px;
}

button:hover {
  background-color: #45a049;
}

span {
  font-size: 24px;
  min-width: 50px;
}
</style>
