<script setup>
function saluda() {
  console.log('Hola')
}

function adios() {
  console.log('Adios')
}
</script>

<template>
  <button @click="saluda">Hola</button>
  <button @click="adios">Adios</button>
</template>
