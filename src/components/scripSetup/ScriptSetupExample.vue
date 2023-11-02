<script setup lang="ts">
import { defineProps, toRefs, defineExpose } from 'vue';
const props = defineProps({
  firstName: {
    type: String,
  },
});

const { firstName } = toRefs(props);

defineExpose({
  firstName
})
</script>

<template>
  <h3>Script Setup</h3>
  <p>{{ firstName }}</p>
</template>

<style scoped></style>
