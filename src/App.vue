<script setup lang="ts">
import { ref } from 'vue';
import Playground from './components/Playground.vue';

const isVisible = ref(true);
</script>

<template>
  <div class="p-5">
    <h1>
      You did it!
      <button class="btn btn-primary btn-sm" @click="isVisible = !isVisible">
        Toggle
      </button>
    </h1>
    <p>
      Visit
      <a href="https://vuejs.org/" target="_blank" rel="noopener">vuejs.org</a>
      to read the documentation
    </p>
    <Playground v-if="isVisible" />
  </div>
</template>

<style scoped></style>