<script setup>

  defineProps(['messages']);
  const emit = defineEmits(['update:messages']);

  function messageEmitted(){
    emit('update:messages', 'Message emitted from child component');
  }  


</script>

<template>



<button @click="messageEmitted()" class="my-10 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Emit Message
</button>
</template>


<style scoped>

</style>