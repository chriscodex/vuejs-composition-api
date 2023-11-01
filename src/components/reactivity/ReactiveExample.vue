<script setup lang="ts">
import { reactive } from 'vue';

// Reactive works with objects
const stateReactive = reactive({
  text: 'Testing',
  counter: 0,
});

setInterval(() => {
  stateReactive.counter++;
}, 500);
</script>

<template>
  <div>
    <p>{{ stateReactive }}</p>
  </div>
</template>

<style scoped></style>
