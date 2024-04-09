<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(true)
</script>

<template>
  <button @click="maVar = 1">- Montrer 1 -</button>
  <button @click="maVar = 2">- Montrer 2 -</button>
  <button @click="maVar = !maVar">- Bascule -</button>
  <h1 v-show="maVar === 1"
  class="text-2xl">En fait au début...</h1>
  <h1 v-show="maVar === 2"
  class="text-2xl">On l'a fait pour la culture</h1>
</template>
