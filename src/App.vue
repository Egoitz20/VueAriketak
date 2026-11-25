<script setup>
import AriketaC3 from './ariketak/03/ariketaC3.vue'
import ariketaC4 from './ariketak/04/ariketaC4.vue'
import AriketaC5 from './ariketak/05/ariketaC5.vue'
// import cabeceraH1 from './components/cabeceraH1.vue'
// import cabeceraNueva from './components/cabeceraNueva.vue'
// import ejemploBoton from './components/ejemploBoton.vue';
const visualizacion = true
</script>

<template>
  <h1>03 Ariketa</h1>
  <div class="A03">
    <ariketaC3 />
    <ariketaC3 />
    <ariketaC3 />
  </div>

  <h1>04 Ariketa</h1>
  <div class="A04">
    <ariketaC4 />
    <ariketaC4 />
    <ariketaC4 />
  </div>

  <h1>05 Ariketa</h1>

  <div class="A05">
    <ariketaC5 v-if="visualizacion" />
  </div>
</template>

<style scoped>
.A03 {
  display: flex;
  flex-wrap: wrap;
}

.A04 {
  display: flex;
  flex-wrap: wrap;
}
</style>
