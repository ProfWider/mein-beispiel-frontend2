<script setup lang="ts">

const items = [
  {
    name: "test",
    price: 42
  },
  {
    name: "test1",
    price: 43
  },
  {
    name: "test2",
    price: 44
  },
  {
    name: "test3",
    price: 45
  },
  {
    name: "test4",
    price: 46
  }
]

</script>

<template>
  <table>
    <thead>
    <tr>
      <th>Name</th>
      <th>Price</th>
    </tr>
    </thead>
    <tbody>
    <tr v-for="item in items" :key="item.price">
      <td>{{item.name}}</td>
      <td>{{item.price}}</td>
    </tr>
    </tbody>
  </table>
</template>
