<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gradient-to-br from-gray-900 via-purple-900 to-indigo-900">

    <!-- Azure Logo -->
    <img src="https://swimburger.net/media/ppnn3pcl/azure.png" alt="Azure Logo" class="mt-8 w-24 h-24" />
    <h2 class="text-4xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-purple-400 mt-10 mb-6 text-center tracking-tight">
      Run on Microsoft Azure
    </h2>
    <h1 class="text-4xl font-light text-gray-200 tracking-wide mb-8">
      Welcome to, <span class="font-semibold text-blue-400">Kim project</span> in Nuxt 3
    </h1>
    <button @click="showModal = true" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-700 transition-colors">
      More details...
    </button>

    <!-- Modal -->
    <div v-if="showModal" class="fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center">
      <div class="bg-gray-800 p-8 rounded-lg shadow-xl max-w-md w-full">
        <h2 class="text-2xl font-semibold mb-4 text-white">Kim apps</h2>
        <p class="mb-4 text-gray-300">Testing only</p>
        <div class="mb-4">
          <h3 class="text-xl font-semibold mb-2 text-blue-400">Run from Azure</h3>
          <p class="text-gray-300">This application is hosted and run on Microsoft Azure, providing scalability, reliability, and performance.</p>
        </div>
        <button @click="showModal = false" class="px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-700 transition-colors">
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