<script setup>
import { ref } from 'vue';
const users = ref([
{
firstName: "firstName",
lastName: "lastName",
email: "firstName@umsa.bo",
role: "Student",
point: 79,
},
{
firstName: "firstName",
lastName: "lastName",
email: "firstName@umsa.bo",
role: "Admin",
point: 99,
},
{
firstName: "firstName",
lastName: "lastName",
email: "firstName@umsa.bo",
role: "Student",
point: 70,
},
{
firstName: "firstName",
lastName: "lastName",
email: "firstName@umsa.bo",
role: "Student",
point: 77,
},
{
firstName: "firstName",
lastName: "lastName",
email: "firstName@umsa.bo",
role: "User",
point: 80,
},
]);
</script>

<template>
  <h2>Vue 3 - Display a list of items width v-for</h2>
  <table>
  <tr>
    <td class="titulo">FIRST NAME</td>
    <td class="titulo">LAST NAME</td>
    <td class="titulo">E-MAIL</td>
    <td class="titulo">ROLE</td>
    <td class="titulo">POINT</td>
    <td class="titulo">New POINT</td>
    <td class="titulo">STATE</td>
  </tr>
  <tr v-for="(user, index) in users" :key="index">
    <div class="dif">{{ user.firstName }}</div>
    <td>{{ user.lastName }}</td>
    <td>{{ user.email }}</td>
    <td>{{ user.role }}</td>
    <td>{{ user.point }}</td>
    <td>
      <div v-if="user.point >= 77" class="color">{{ user.point }}</div>
    </td>
    <td>
      <div v-if="user.point >= 77" class="color">{{ user.role }} ROLE</div>
    </td>
  </tr>
 </table>
</template>

<style scoped>
table{
  width: 1200px;
  border: 1px solid rgb(131, 185, 250);
  color: rgb(199, 171, 222);
}
.color{
 
  color: rgb(255, 0, 0);
  
}
.titulo{
  
  text-align: left;
  color: black;
  font-size: 20px;
  background: #7e60ca;
  border-radius: 15px 15px 15px 15px;
}

</style>