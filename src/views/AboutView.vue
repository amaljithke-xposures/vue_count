<script setup>
import { ref } from 'vue'

// Single count for both increment and decrement
const count = ref(0)

// Function to increase the count
const increase = () => {
  count.value++
}

// Function to decrease the count
const decrease = () => {
  count.value--
}
</script>

<template>
  <div class="counter-container">
    <h2>Counter Section</h2>
    <div class="counter">
      <!-- Decrease Button -->
      <button @click="decrease">-</button>
      
      <!-- Current count value -->
      <span>{{ count }}</span>
      
      <!-- Increase Button -->
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
