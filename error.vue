<!-- pages/error.vue or error.vue in root -->
<script setup lang="ts">
defineProps({
  error: Object
});
</script>

<template>
  <div class="surface-ground flex align-items-center justify-content-center min-h-screen min-w-screen overflow-hidden">
    <div class="flex flex-column align-items-center justify-content-center">
      <img src="/images/logo-dark.svg" alt="Logo" class="mb-5 w-6rem flex-shrink-0">
      <div
        style="border-radius:56px; padding:0.3rem; background: linear-gradient(180deg, rgba(233, 30, 99, 0.4) 10%, rgba(33, 150, 243, 0) 30%);"
      >
        <div
          class="w-full surface-card py-8 px-5 sm:px-8 flex flex-column align-items-center"
          style="border-radius:53px"
        >
          <span class="text-blue-500 font-bold text-3xl">404</span>
          <h1 class="text-900 font-bold text-5xl mb-2">
            Not Found
          </h1>
          <div class="text-600 mb-5">
            Requested resource is not available
          </div>
          <NuxtLink
            to="/"
            class="w-full flex align-items-center py-5 border-300 border-bottom-1"
          >
            <span
              class="flex justify-content-center align-items-center bg-cyan-400 border-round"
              style="height:3.5rem; width:3.5rem;"
            >
              <i class="pi pi-home text-50 text-2xl" />
            </span>
            <span class="ml-4 flex flex-column">
              <span class="text-900 lg:text-xl font-medium mb-1">Go to Dashboard</span>
              <span class="text-600 lg:text-lg">Back to main page</span>
            </span>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>
