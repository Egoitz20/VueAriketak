<script setup>
const formularioBloqueado = true
const clase = 'berdea'
const estaConectado = true
const edad = 20
const nombres = ['Alice', 'Bob', 'Carol', 'David']
const usuarios = [
  { id: 1, nombre: 'Ane' },
  { id: 2, nombre: 'Mikel' },
  { id: 3, nombre: 'Jon' }
]
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
  <!-- For normal -->
  <ul>
    <li v-for="nombre in nombres">
      {{ nombre }}
    </li>
  </ul>

  <!-- For asociado a id -->
  <ul>
    <li v-for="usuario in usuarios" :key="usuario.id">
      {{ usuario.nombre }}
    </li>
  </ul>
</template>

<style scoped>
.berdea {
  color: green;
}

.gorria {
  color: red;
}
</style>
