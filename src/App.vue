<script setup>
import { ref } from 'vue'; // Tambahkan ref untuk reactive data

const count = ref(0); // Inisialisasi counter

function increment() {
  count.value++; // Fungsi untuk menambah counter
}
</script>

<template>
  <div>
    <p>Counter: {{ count }}</p>
    <button @click="increment">Tambah</button>
  </div>
</template>

<style scoped>
/* Tambahkan gaya sesuai kebutuhan */
div {
  text-align: center;
  margin-top: 2rem;
}

button {
  padding: 0.5rem 1rem;
  font-size: 1rem;
  cursor: pointer;
}
</style>
