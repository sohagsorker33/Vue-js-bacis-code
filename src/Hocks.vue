
 <script setup>
   import { ref,onMounted } from 'vue';

   let user=ref([]);

   function getUser(){
     user.value=[{name:"sohag",id:1},{name:"ali",id:2}]
   }
   onMounted(()=>{
    console.log("mounted");
     getUser();
   })
</script>

<template>
  <div v-for="(user, index) in user" :key='index'>{{ user.name }}</div>
</template>