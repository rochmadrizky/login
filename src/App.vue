<script setup>
import BtnLogin from "./components/BtnLogin.vue";
import InputBox from "./components/InputBox.vue";
</script>

<template>
  <div class="min-h-screen flex items-center justify-center bg-gray-100">
    <div class="bg-white p-8 shadow-md rounded-md w-96">
      <h1 class="text-3xl font-semibold mb-4">Login?</h1>
      <form @submit.prevent="login">
        <InputBox
          type="text"
          label="Username"
          id="username"
          placeholder="Your username"
        />
        <InputBox
          type="password"
          label="Password"
          id="password"
          placeholder="Your password"
        />
        <BtnLogin>Login</BtnLogin>
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
