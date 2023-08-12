<script setup lang="ts">
import { ref } from 'vue';
import Counter from './components/Counter.vue';

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
