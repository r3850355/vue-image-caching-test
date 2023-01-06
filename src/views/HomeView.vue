<script setup>
import { ref } from 'vue'
// import TheWelcome from '../components/TheWelcome.vue'
let random = ref(0)
random.value = Math.floor(Math.random() * 99999)
</script>

<template>
  <main>
    <!-- <TheWelcome /> -->
    <h1>Home Page</h1>
    <img src="https://vitejs.dev/logo-with-shadow.png" style="width:150px">
    <img :src="`https://vitejs.dev/logo-with-shadow.png?something=${random}`" style="width:150px">
    <img src="https://vitejs.dev/logo-with-shadow.png?otherthing=123" style="width:150px">
  </main>
</template>
