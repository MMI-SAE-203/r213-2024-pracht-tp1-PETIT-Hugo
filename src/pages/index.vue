<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(true)
</script>

<template>
  <p>la variable vaut : {{ maVar }}</p>
  <button @click="maVar = maVar === 1 ? 0 : 1">Montrer 1</button>

  <button @click="maVar = maVar === 2 ? 0 : 2">Montrer 2</button>

  <button @click="maVar = !maVar">Cacher</button>


  <h1 v-show="maVar === 1"
  class="text-2xl">En fait au début...</h1>

  <h1 v-show="maVar === 2"
  class="text-2xl">On l'a fait pour la culture</h1>

  <img v-show="maVar === 1 || 2" src="https://www.aufoindelarue.com/wp-content/uploads/2024/01/La-Feve.jpg">


</template>
