<script setup>
import childComponent from './childComponent.vue';
defineProps (['message']);

</script>

<template>
   
 <div class="parentComponent">
    <h1 class="font-2xl" >{{ message.message }}</h1>
    
    <childComponent v-model:messages="message.message" /> 
  </div>

</template>

<style scoped></style>