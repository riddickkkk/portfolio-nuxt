<script setup lang="ts">
const props = defineProps({
  error: Object
})

const handleError = () => clearError({ redirect: '/' })
</script>

<template>
  <div class="min-h-screen bg-[#182615] text-[#fdfbf7] flex flex-col items-center justify-center p-4 text-center">
    <h1 class="text-8xl font-black text-[#a3b18a] mb-2">404</h1>
    <h2 class="text-2xl font-bold mb-4">Page Not Found</h2>
    <p class="text-[#dad7cd] mb-6 max-w-md">
      The requested page could not be found.
    </p>
    <button 
      @click="handleError" 
      class="px-6 py-2.5 bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] rounded-full text-xs font-bold uppercase transition-all shadow-md cursor-pointer"
    >
      Back to Home
    </button>
  </div>
</template>