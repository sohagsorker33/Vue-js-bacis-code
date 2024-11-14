
<script setup>
 import { ref,reactive } from 'vue';
/*  let email=ref("")
  let password=ref("") */

const from=reactive({
  email:"",
  password:""

});
</script>

<template>

<div>
  <form action="">
    <input type="text" name="email" placeholder="Enter email" v-model="from.email">
    <input type="text" name="email" placeholder="Enter email" v-model="from.password">
  </form>
</div>
<!-- ref ar jonno
 {{ email }}/{{ password }}  -->

 {{ from }}
</template>