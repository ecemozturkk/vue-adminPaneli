<template>
  <div>
    <!-- Breadcrumb -->
    <Breadcrumb breadcrumb="Blank" />

    <div class="mt-8">
      <h4 class="text-gray-600" style="font-size:40px;">İletişim</h4>

      <div class="mt-4">
        <div class="p-6 bg-white rounded-md shadow-md">
          <h2 class="text-lg font-semibold text-gray-700 capitalize">
            Account settings
          </h2>

          <form @submit.prevent="register">
            <div class="grid grid-cols-1 gap-6 mt-4 sm:grid-cols-2">
              <div>
                <label class="text-gray-700" for="username">Username</label>
                <input
                  class="
                    w-full
                    mt-2
                    border-gray-200
                    rounded-md
                    focus:border-indigo-600
                    focus:ring
                    focus:ring-opacity-40
                    focus:ring-indigo-500
                  "
                  type="text"
                  v-model="user.username"
                />
              </div>

              <div>
                <label class="text-gray-700" for="emailAddress"
                  >Email Address</label
                >
                <input
                  class="
                    w-full
                    mt-2
                    border-gray-200
                    rounded-md
                    focus:border-indigo-600
                    focus:ring
                    focus:ring-opacity-40
                    focus:ring-indigo-500
                  "
                  type="email"
                  v-model="user.email"
                />
              </div>

              <div>
                <label class="text-gray-700" for="password">Password</label>
                <input
                  class="
                    w-full
                    mt-2
                    border-gray-200
                    rounded-md
                    focus:border-indigo-600
                    focus:ring
                    focus:ring-opacity-40
                    focus:ring-indigo-500
                  "
                  type="password"
                  v-model="user.password"
                />
              </div>

              <div>
                <label class="text-gray-700" for="passwordConfirmation"
                  >Password Confirmation</label
                >
                <input
                  class="
                    w-full
                    mt-2
                    border-gray-200
                    rounded-md
                    focus:border-indigo-600
                    focus:ring
                    focus:ring-opacity-40
                    focus:ring-indigo-500
                  "
                  type="password"
                  v-model="user.confirm"
                />
              </div>
            </div>

            <div class="flex justify-end mt-4">
              <button
                class="
                  px-4
                  py-2
                  text-gray-200
                  bg-gray-800
                  rounded-md
                  hover:bg-gray-700
                  focus:outline-none focus:bg-gray-700
                "
              >
                Save <!-- onclick vs tarzi atama yapilmali -->
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>


































<script setup lang="ts">
import { ref } from 'vue'
import Breadcrumb from "../partials/Breadcrumb.vue";
interface User {
  username: string
  email: string
  password: string
  confirm: string
}

const user = ref<User>({
  username: '',
  email: '',
  password: '',
  confirm: '',
})

const register = () => {
  const data = JSON.parse(JSON.stringify(user.value))
  console.log('Registered: ', data)
}
</script>
