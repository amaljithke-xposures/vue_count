<script setup>
import { ref } from 'vue'

const count = ref(0)

const increase = () => {
  count.value++
}

const decrease = () => {
  count.value--
}
</script>

<template>
  <div class="counter-container">
    <h1>Vue Counter</h1>
    <div class="counter">
      <button @click="decrease">-</button>
      <span>{{ count }}</span>
      <button @click="increase">+</button>
    </div>
  </div>
</template>

<style scoped>
.counter-container {
  text-align: center;
  margin-top: 50px;
}

.counter {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
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
