<script setup>
import { ref , reactive , provide } from 'vue';
import parentComponent from './components/parentComponent.vue';
const message = reactive({ 
  message: 'Hello World!',
  seen: true,
  }); 
</script>

<template>
  <div id="app">
    <parentComponent :message="message" />

    
  </div>
</template>

<style scoped>

</style>
