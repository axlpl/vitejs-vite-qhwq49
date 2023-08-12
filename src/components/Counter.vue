<script setup lang="ts">
import { ref } from 'vue';

const value = ref<number>(0);
</script>

<template>
  <div class="content">
    <button @click="value += 1">+</button>
    <h2>Counter: {{ value }}</h2>
  </div>
</template>
