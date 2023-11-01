<script setup lang='ts'>
import { inject } from 'vue';

const username = inject('username');
</script>

<template>
  <div>
    <p>Username: {{ username }}</p>
  </div>
</template>

<style scoped>

</style>