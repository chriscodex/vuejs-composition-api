<script setup lang="ts">
import { ref, watch } from 'vue';

const btn = ref(null);

watch(btn, () => {
  console.log(btn.value);
});
</script>

<template>
  <div>
    <h3>Template Ref</h3>
    <button ref="btn">Click</button>
  </div>
</template>

<style scoped></style>
