<script setup>
import { ref } from 'vue';
const count = ref(0)
</script>

<template>
  <div class="container">
    <h1>Counter</h1>
    <p class="count">{{count}}</p>
    <div class="buttons">
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </div>
</template>

<style scoped>
  .container{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 100vw;
    flex-direction: column;
    gap: 50px;
  }
  .count{
    font-size: 72px;
    font-weight: bold;
  }
  .buttons{
    display: flex;
    align-items: center;
    gap: 10px;
  }
  button{
    width: 40px;
    padding: 10px;
    font-size: 28px;
    cursor: pointer;
  }
</style>
