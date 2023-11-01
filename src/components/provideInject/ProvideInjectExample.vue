<script setup lang='ts'>
import { provide } from 'vue';
import ChildC from './ChildC.vue';

provide('username', 'Christian')

</script>

<template>
  <div>
    <h3>Provide Inject</h3>
    <ChildC />
  </div>
</template>

<style scoped>

</style>