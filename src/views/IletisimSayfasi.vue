<template>
  <div>
    <!-- Breadcrumb -->
    <!-- <Breadcrumb breadcrumb="Tables" /> -->

    <div class="mt-4">
      <h4 class="text-black-600">KATEGORILER</h4>

      <div class="mt-6">
        <div class="my-6 overflow-hidden bg-white rounded-md shadow">
          <table class="w-full text-left border-collapse">
            <thead class="border-b">
              <tr>
                <th
                  class="px-5 py-3 text-sm font-medium text-gray-100 uppercase bg-indigo-800"
                >
                  Kategori ID
                </th>
                <th
                  class="px-5 py-3 text-sm font-medium text-gray-100 uppercase bg-indigo-800"
                >
                  Kategori Adi
                </th><th
                  class="px-5 py-3 text-sm font-medium text-gray-100 uppercase bg-indigo-800"
                >
                  Kategorinin Urunleri
                </th>
              </tr>
            </thead>
            <tbody>
              <tr
                v-for="category in categories" :key="category.categoryId"
                class="hover:bg-gray-200"
              >
                <td class="px-6 py-4 text-lg text-gray-700 border-b">
                  {{ category.categoryId }}
                </td>
                <td class="px-6 py-4 text-gray-500 border-b">
                  {{ category.categoryName }}
                </td>
                <td class="px-6 py-4 text-gray-500 border-b">
                  {{ category.products }}
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

   

    
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from "vue";
import axios from "axios";
import { useTableData } from '../hooks/useTableData'
const { simpleTableData, paginatedTableData, wideTableData } = useTableData()

//import Breadcrumb from '../partials/Breadcrumb.vue'
const categories = ref([]);
onMounted(async () => {
  await axios
    .get("https://localhost:44358/api/CustomerMessage")
    .then((response) => {
      categories.value = response.data;
    });
  console.log(categories);
});
</script>
