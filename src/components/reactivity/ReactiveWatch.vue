<script setup lang="ts">
import { reactive, watch } from 'vue';

// Reactive works with objects
const stateReactive = reactive({
  text: 'Testing',
  counter: 0,
});

setInterval(() => {
  stateReactive.counter++;
}, 500);

watch(() => stateReactive.counter, (newValue, oldValue) => {
  console.log(newValue, oldValue);
})
</script>

<template>
  <div>
    <p>{{ stateReactive }}</p>
  </div>
</template>

<style scoped></style>
