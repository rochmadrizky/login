<template>
  <div class="mb-4">
    <label
      class="block text-gray-600 text-sm font-medium mb-2"
      for="username"
      >{{ props.label }}</label
    >
    <input
      :type="props.type"
      v-model="username"
      :id="props.id"
      name="username"
      class="w-full px-3 py-2 border rounded-md"
      :placeholder="props.placeholder"
    />
  </div>
</template>

<script setup>
const props = defineProps({
  type: String,
  placeholder: String,
  label: String,
});
</script>
