<script setup lang="ts">
import { ref } from 'vue';
import Counter from './components/Counter.vue';

// v-model, which means two-way binding.
// Do not modify the App.js file.
// We must enable v-model between App and Counter.

const value = ref<number>(0);
</script>

<template>
  <Counter v-model="value" />
  <hr />
  <div class="content">
    <button @click="value += 1">+</button>
    <h2>App: {{ value }}</h2>
  </div>
  <hr />
  <input v-model.number="value" />
</template>
