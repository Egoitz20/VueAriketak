<script setup>
const formularioBloqueado = true
const clase = 'berdea'
const estaConectado = true
const edad = 20
</script>
<template>
  <button :disabled="formularioBloqueado" :class="clase">Enviar</button>
  <!-- Si es true, aparece; si es false, desaparece -->
  <h2 v-if="estaConectado">Control de edad</h2>
  <!-- Empieze bloque if -->
  <p v-if="edad < 10">Menor de 10</p>
  <p v-else-if="edad < 18">Menor de 18</p>
  <p v-else-if="edad < 35">Menor de 35</p>
  <p v-else>Mayor de 65</p>
  <!-- Fin bloque if -->
</template>

<style scoped>
.berdea {
  color: green;
}

.gorria {
  color: red;
}
</style>
