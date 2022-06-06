<template>
  <div>
    <!-- Breadcrumb -->
    <!-- <Breadcrumb breadcrumb="Contact" /> -->
    <table class="table">
      <thead>
        <tr>
          <th scope="col">ID</th>
          <th scope="col">Name</th>
          <th scope="col">Image</th>
          <th scope="col">Stock</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="product in products" :key="product.productId">
          <th scope="row">{{ product.productId }}</th>
          <td>{{ product.productName }}</td>
          <td>{{ product.productImage }}</td>
          <td>{{ product.stock }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from "vue";
import axios from "axios";

// import Breadcrumb from "../partials/Breadcrumb.vue";

const products = ref([]);
onMounted(async () => {
  await axios
    .get("http://kozmosapi-001-site1.itempurl.com/api/Products")
    .then((response) => {
      products.value = response.data;
    });
  console.log(products);
});

//composition API

const open = ref(false);
</script> 


