<template>
  <div class="min-h-screen flex items-center justify-center bg-gradient-to-br from-green-50 to-green-200">
    <div class="bg-white rounded-2xl shadow-2xl p-10 max-w-xl w-full text-center space-y-6">
      
      <!-- Título -->
      <h1 class="text-5xl font-bold text-green-700">SmartBins</h1>

      <!-- Descripción -->
      <p class="text-gray-600 text-lg">
        Bienvenido a SmartBins, el sistema de monitoreo de residuos,
        analiza las canecas en tiempo real y mejora la eficiencia de la recolección.
      </p>

      <!-- Caneca animada (opcional) -->
      <div class="flex justify-center">
        <svg class="w-20 h-20 text-green-600 dark:text-green-400 animate-bounce-slow" fill="currentColor" viewBox="0 0 24 24">
          <path d="M9 3a3 3 0 0 1 6 0h5a1 1 0 1 1 0 2h-1l-1.2 14.4A3 3 0 0 1 14.8 22H9.2a3 3 0 0 1-2.999-2.6L5 5H4a1 1 0 1 1 0-2h5Zm2 5a1 1 0 0 0-2 0v8a1 1 0 1 0 2 0V8Zm4-1a1 1 0 1 0-2 0v8a1 1 0 0 0 2 0V7Z" />
        </svg>
      </div>

      <!-- Botones -->
      <div class="flex justify-center space-x-4">
        <Link
          href="/login"
          class="bg-green-600 hover:bg-green-700 text-white font-semibold py-2 px-6 rounded-lg transition"
        >
          Iniciar sesión
        </Link>

        <Link
          href="/register"
          class="bg-green-100 hover:bg-green-200 text-green-800 font-semibold py-2 px-6 rounded-lg border border-green-300 transition"
        >
          Registrarse
        </Link>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { Link } from '@inertiajs/vue3';
</script>

<style scoped>
@keyframes bounce-slow {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}
.animate-bounce-slow {
  animation: bounce-slow 2s infinite;
}
</style>

