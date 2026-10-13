<script lang="ts" setup>
import { onMounted, onUnmounted, ref } from 'vue';
 
const count = ref(1);
 
onMounted(() => {
  console.log('onMounted');
});
 
onUnmounted(() => {
  console.log('onUnmounted');
});
</script>

<template>
  <h2>Playground for Kids</h2>
  <button class="btn btn-primary" @click="count++">
    Increment ({{ count }})
  </button>
</template>

<style lang="css" scoped></style>