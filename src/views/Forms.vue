<template>
  <div>
    <!-- Breadcrumb -->
    <!-- <Breadcrumb breadcrumb="Forms" /> -->

    <div class="mt-4">
      <h4 class="text-gray-600">Model Form</h4>

      <div class="mt-4">
        <div
          class="
            w-1/2
            max-w-sm
            overflow-hidden
            bg-white
            border
            rounded-md
            shadow-md
          "
        >
          <div style="float: right">
            <form>
              <div
                class="
                  flex
                  items-center
                  justify-between
                  px-5
                  py-3
                  text-gray-700
                  border-b
                "
              >
                <h3 class="text-sm">Kategori Ekle</h3>
                <button>
                  <svg
                    class="w-4 h-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M6 18L18 6M6 6l12 12"
                    />
                  </svg>
                </button>
              </div>

              <div class="px-5 py-6 text-gray-700 bg-gray-200 border-b">
                <label class="text-xs">Kategori Adi :</label>

                <div class="relative mt-2 rounded-md shadow-sm">
                  <span
                    class="
                      absolute
                      inset-y-0
                      left-0
                      flex
                      items-center
                      pl-3
                      text-gray-600
                    "
                  >
                    <svg
                      class="w-6 h-6"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 00-1-1H4a2 2 0 110-4h1a1 1 0 001-1V7a1 1 0 011-1h3a1 1 0 001-1V4z"
                      />
                    </svg>
                  </span>

                  <input
                    type="text"
                    class="
                      w-full
                      px-12
                      py-2
                      border-transparent
                      rounded-md
                      appearance-none
                      focus:border-indigo-600
                      focus:ring
                      focus:ring-opacity-40
                      focus:ring-indigo-500
                    "
                  />
                </div>
              </div>

              <div class="flex items-center justify-between px-5 py-3">
                <button
                  class="
                    px-3
                    py-1
                    text-sm text-gray-700
                    bg-gray-200
                    rounded-md
                    hover:bg-gray-300
                    focus:outline-none
                  "
                >
                  Iptal
                </button>
                <button
                  class="
                    px-3
                    py-1
                    text-sm text-white
                    bg-indigo-600
                    rounded-md
                    hover:bg-indigo-500
                    focus:outline-none
                  "
                >
                  Ekle
                </button>
              </div>
            </form>
          </div>
        </div>
        <div
          class="
            w-1/2
            max-w-sm
            overflow-hidden
            bg-white
            border
            rounded-md
            shadow-md
          "
        >
          <form>
            <div
              class="
                flex
                items-center
                justify-between
                px-5
                py-3
                text-gray-700
                border-b
              "
            >
              <h3 class="text-sm">Kategori Sil</h3>
              <button>
                <svg
                  class="w-4 h-4"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M6 18L18 6M6 6l12 12"
                  />
                </svg>
              </button>
            </div>

            <div class="px-5 py-6 text-gray-700 bg-gray-200 border-b">
              <label class="text-xs">Kategori Adi</label>

              <div class="relative mt-2 rounded-md shadow-sm">
                <span
                  class="
                    absolute
                    inset-y-0
                    left-0
                    flex
                    items-center
                    pl-3
                    text-gray-600
                  "
                >
                  <svg
                    class="w-6 h-6"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 00-1-1H4a2 2 0 110-4h1a1 1 0 001-1V7a1 1 0 011-1h3a1 1 0 001-1V4z"
                    />
                  </svg>
                </span>

                <input
                  type="text"
                  class="
                    w-full
                    px-12
                    py-2
                    border-transparent
                    rounded-md
                    appearance-none
                    focus:border-indigo-600
                    focus:ring
                    focus:ring-opacity-40
                    focus:ring-indigo-500
                  "
                />
              </div>
            </div>

            <div class="flex items-center justify-between px-5 py-3">
              <button
                class="
                  px-3
                  py-1
                  text-sm text-gray-700
                  bg-gray-200
                  rounded-md
                  hover:bg-gray-300
                  focus:outline-none
                "
              >
                Iptal
              </button>
              <button
                class="
                  px-3
                  py-1
                  text-sm text-white
                  bg-red-600
                  rounded-md
                  hover:bg-indigo-500
                  focus:outline-none
                "
              >
                Sil
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
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
    .get("http://kozmosapi-001-site1.itempurl.com/api/Categories")
    .then((response) => {
      categories.value = response.data;
    });
  console.log(categories);
});

// import { ref } from "vue";
// //import Breadcrumb from '../partials/Breadcrumb.vue'

// interface User {
//   username: string;
//   email: string;
//   password: string;
//   confirm: string;
// }

// const user = ref<User>({
//   username: "",
//   email: "",
//   password: "",
//   confirm: "",
// });

// const register = () => {
//   const data = JSON.parse(JSON.stringify(user.value));
//   console.log("Registered: ", data);
// };
</script>