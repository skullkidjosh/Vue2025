<template>
<h1>Ejemplo de Reactividad</h1>
<p>{{ contador }}</p>
<button @click="Incrementar">Incrementar cuenta</button>
<button @click="Decrementar">Decrementar cuenta</button>
<button @click="Eliminar">Eliminar cuenta</button>
  </template>

<script setup>
import {ref} from 'vue';
const contador = ref(1);
const Incrementar = () => {
  contador.value++;
}

const Decrementar = () => {
  contador.value--;
}

const Eliminar = () => {
  contador.value=0;
}

</script>

<style scoped>
p {
  color: rgb(146, 26, 26);
  text-align: center;
}

h1 {
  color: rgb(150, 207, 133);
  text-align: center;
}
</style>
