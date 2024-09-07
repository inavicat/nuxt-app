<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gradient-to-br from-gray-900 via-purple-900 to-indigo-900 px-4 sm:px-6 lg:px-8">

    <!-- Azure Logo -->
    <img src="https://swimburger.net/media/ppnn3pcl/azure.png" alt="Azure Logo" class="mt-8 w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24" />
    <h2 class="text-2xl sm:text-3xl md:text-4xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-purple-400 mt-6 sm:mt-8 md:mt-10 mb-4 sm:mb-5 md:mb-6 text-center tracking-tight">
      Run from Microsoft Azure
    </h2>
    <h1 class="text-2xl sm:text-3xl md:text-4xl font-light text-gray-200 tracking-wide mb-6 sm:mb-7 md:mb-8 text-center">
      Welcome to, <span class="font-semibold text-blue-400">Kim project</span> in Nuxt 3
    </h1>
    <button @click="showModal = true" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-700 transition-colors text-sm sm:text-base">
      More details...
    </button>

    <!-- Modal -->
    <div v-if="showModal" class="fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center p-4">
      <div class="bg-gray-800 p-6 sm:p-8 rounded-lg shadow-xl max-w-xs sm:max-w-sm md:max-w-md w-full">
        <h2 class="text-xl sm:text-2xl font-semibold mb-3 sm:mb-4 text-white">Kim apps</h2>
        <p class="mb-3 sm:mb-4 text-gray-300 text-sm sm:text-base">Testing only</p>
        <div class="mb-4">
          <h3 class="text-lg sm:text-xl font-semibold mb-2 text-blue-400">Run from Azure</h3>
          <p class="text-gray-300 text-sm sm:text-base">This application is hosted and run on Microsoft Azure, providing scalability, reliability, and performance.</p>
        </div>
        <button @click="showModal = false" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-700 transition-colors text-sm sm:text-base">
          Close Modal
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const showModal = ref(false)
</script>