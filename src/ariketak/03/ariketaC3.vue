<script setup></script>

<template>
  <div class="producto">
    <h2>Sobremesa</h2>
    <p>Ordenador de sobremesa</p>
    <p>45€</p>
    <button>Comprar</button>
  </div>
</template>

<style scoped>
.producto {
  width: 200px;
  padding: 16px;
  margin: 10px;
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  background-color: #ffffff;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
  display: flex;
  flex-direction: column;
  gap: 8px;
  font-family: sans-serif;
}

h2 {
  margin: 0;
  font-size: 18px;
  color: #2e7d32;
}

p {
  margin: 0;
  font-size: 14px;
  color: #555;
}

p:last-of-type {
  font-size: 18px;
  font-weight: bold;
  color: #111;
  margin-top: 4px;
}

button {
  margin-top: auto;
  padding: 8px 12px;
  border: none;
  border-radius: 6px;
  background-color: #2e7d32;
  color: white;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
}

button:hover {
  background-color: #1b5e20;
}
</style>
