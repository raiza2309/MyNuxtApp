<script setup lang="ts">
const state = ref<boolean>(true)
</script>
<template>
  <div>
    <!-- <NuxtWelcome /> -->
    <h1>{{ state }}</h1>
    <button class="mx-4 btn" @click="state = !state">
      Change state
    </button>
    <NuxtLink :to="{ name: 'about' }" class="text-sky-500 hover:text-sky-700">
      Go To Index
    </NuxtLink>
  </div>
</template>
<style scoped>
  .btn {
    @apply bg-blue-600 text-white px-4 py-2 rounded-tl-xl rounded-br-lg rounded-tr-sm rounded-bl-sm hover:bg-blue-500 duration-300 block;
  }
</style>
