<script setup>
   let friends=['Sohag','Ashraful',"Sujon","Rofikul"];
   const products=[
    {
     name:"T-Shart",
     description:"T-Shart is the best quelity",
     price:400
    },
    {
     name:"Jinset Pant",
     description:"Jinset Pant is the best quelity",
     price:500
    }
   ];
</script>
   
<template>
  <div>
    <ul>
     <li v-for="(item, index) in friends" :key='index' >{{ item }}</li>
     <hr> 
    <li v-for="(item, index) in friends" :key='index' >{{ index }} {{ item }}</li>
    </ul>
    <hr>
    <h3>Product Table</h3>
    <table>
      <tr>
        <th>Name</th>
        <th>Description</th>
        <th>Price</th>
      </tr>
        <tr v-for="(product, index) in products" :key='index' >
          <td>{{ product.name }}</td>
          <td>{{ product.description }}</td>
          <td>{{ product.price }}</td>
        </tr>
    </table> 
  </div>
</template>

<style>

table, td, th {
  border: 1px solid black;
  text-align: center;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  height: 70px;
}
</style>