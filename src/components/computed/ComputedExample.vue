<script setup lang='ts'>
import { ref, computed } from 'vue';

const firstName = ref('Christian')
const lastName = ref('Espinoza')

const fullName = computed(() => {
  return `${firstName.value} ${lastName.value}`
})

</script>

<template>
  <div>
    <h3>Computed</h3>
    <p>Fullname: {{ fullName }}</p>
  </div>
</template>

<style scoped>

</style>