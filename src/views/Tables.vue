<template>
  <div class="flex justify-center items-center">
    <!-- Breadcrumb -->
    <!-- <Breadcrumb breadcrumb="Tables" /> -->

    <div class="mt-100 mb-100 ">
      <div class="p-3 bg-white shadow rounded-lg max-w-xl mt-10">
      
        <h4 class=" mt-2 text-center text-xl text-black-500 font-bold">KOZMOZ Admin</h4>
        <div class="text-center">
        <span
            class="mt-3 inline-block px-3 py-1 mb-2 mr-2 text-sm font-semibold text-black-700 bg-blue-300 rounded-full"
            >{{siteInfo.keyWords}}</span
          >
          </div>
      </div>

      <div class=" max-w-xl mt-10 overflow-hidden justife-center bg-white rounded shadow-lg ">

        <div class="px-7 py-4">
          <div class="text-center mb-2 text-xl font-bold text-gray-900">
            {{siteInfo.siteName}}
          </div>
          <p class="text-base text-gray-700">
            Kozmos Sitesi sanatla alakalı istediğiniz ürünleri bulabileceğiniz bir e-ticaret sitesidir.
          </p>
          
        </div>
        <div class="px-6 pt-4 pb-2">
          
          <span
            class="inline-block px-3 py-1 mb-2 mr-2 text-sm font-semibold text-black-700 bg-blue-500 rounded-full"
            >{{siteInfo.facebookUrl}}</span
          >
          <span
            class="inline-block px-3 py-1 mb-2 mr-2 text-sm font-semibold text-black-700 bg-blue-500 rounded-full"
            >{{siteInfo.instagramUrl}}</span
          >
          <span
            class="inline-block px-3 py-1 mb-2 mr-2 text-sm font-semibold text-black-700 bg-blue-500 rounded-full"
            >{{siteInfo.linkedinUrl}}</span
          >
        </div>

      </div>
    </div>
    




  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from "vue";
import axios from "axios";



//import Breadcrumb from '../partials/Breadcrumb.vue'
const siteInfo = ref({
  phoneNumber: "",
  description: "",
  keyWords: "",
  facebookUrl: "",
  instagramUrl: "",
  linkedinUrl: "",
  siteName: "",
});
onMounted(async () => {
  await axios
    .get("http://kozmosapi-001-site1.itempurl.com/api/SiteInfo")
    .then((response) => {
      console.log(response.data)
      siteInfo.value = response.data;
    });

});
</script>