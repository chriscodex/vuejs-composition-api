<script setup lang="ts">
import { computed, toRefs } from 'vue';

const { firstName, lastName } = toRefs(
  defineProps({
    firstName: {
      type: String,
    },
    lastName: {
      type: String,
    },
  })
);

const fullName = computed(() => {
  return `${firstName} ${lastName}`;
});
</script>

<template>
  <div>
    <h3>Props</h3>
    <p>Fullname: {{ fullName }}</p>
  </div>
</template>

<style scoped></style>
