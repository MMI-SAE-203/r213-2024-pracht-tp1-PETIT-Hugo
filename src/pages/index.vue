<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(true)
</script>

<template>
  <button @click="maVar = false">- Cacher -</button>
  <button @click="maVar = true">- Montrer -</button>
  <button @click="maVar = !maVar">- Bascule -</button>
  <h1 v-show="maVar"
  class="text-2xl">En fait au début...</h1>
</template>
