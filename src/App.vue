<script setup>
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div class="min-h-screen flex items-center justify-center bg-gray-100">
    <div class="bg-white p-8 shadow-md rounded-md w-96">
      <h1 class="text-3xl font-semibold mb-4">Login?</h1>
      <form @submit.prevent="login">
        <div class="mb-4">
          <label
            class="block text-gray-600 text-sm font-medium mb-2"
            for="username"
            >Username</label
          >
          <input
            type="text"
            v-model="username"
            id="username"
            name="username"
            class="w-full px-3 py-2 border rounded-md"
            placeholder="Your username"
          />
        </div>
        <div class="mb-6">
          <label
            class="block text-gray-600 text-sm font-medium mb-2"
            for="password"
            >Password</label
          >
          <input
            type="password"
            v-model="password"
            id="password"
            name="password"
            class="w-full px-3 py-2 border rounded-md"
            placeholder="Your password"
          />
        </div>
        <div class="mb-2">
          <button
            type="submit"
            class="w-full bg-blue-500 text-white py-2 px-4 rounded-md hover:bg-blue-600 focus:outline-none focus:ring focus:ring-blue-400"
          >
            Login
          </button>
        </div>
      </form>
      <div class="text-center mb-4">
        <a href="#" class="text-sm text-blue-500">Forgot your password?</a>
      </div>
      <div class="text-center">
        <p class="text-gray-600 text-sm">
          Don't have an account? <a href="#" class="text-blue-500">Sign up</a>
        </p>
      </div>
    </div>
  </div>
</template>
