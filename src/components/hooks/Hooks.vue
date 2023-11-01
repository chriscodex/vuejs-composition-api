<script setup lang="ts">
import { onBeforeMount, onMounted } from 'vue';

const text = 'Testing Hooks';

onBeforeMount(() => {
  console.log('onBeforeMount');
})

onMounted(() => {
  console.log('onMounted');
})
</script>

<template>
  <div>
    <p>{{ text }}</p>
  </div>
</template>

<style scoped></style>
