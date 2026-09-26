<script setup lang="ts">
import { ref } from 'vue'

const contador = ref(0)

function sumar() {
  contador.value = contador.value + 1
}

function restar() {
  contador.value = contador.value - 1
}
</script>

<template>
  <div class="contenedor-principal">
    <h1>Contador</h1>
    
    <h2>Valor: {{ contador }}</h2>
    
    <button @click="sumar">más +</button>
    <button @click="restar">menos -</button>
  </div>
</template>

<style scoped>
.contenedor-principal {
  text-align: center;
  margin-top: 50px;
  font-family: Arial, sans-serif;
}

button {
  margin: 10px;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}
</style>