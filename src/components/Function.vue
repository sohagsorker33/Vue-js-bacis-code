 <script setup>
import { ref, reactive } from 'vue';

let number=ref(0);

function increment(){
   number.value++
}
function decrement(){
   number.value--
}
</script>

<template>
   
    <button @click="increment">Increment</button>
    {{ number }}
    <button @click="decrement">Decrement</button>
</template>
<style scoped>

</style>

 
