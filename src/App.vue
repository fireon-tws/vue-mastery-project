<script setup lang="ts">
import { RouterView, RouterLink } from 'vue-router'
</script>

<template>
  <header class="p-6 bg-white border-b border-slate-200 shadow-sm">
    <nav class="max-w-4xl mx-auto flex justify-between items-center">
      <h1 class="text-xl font-bold text-brand-600">MyDev Showcase</h1>
      <div class="space-x-4">
        <RouterLink to="/" class="hover:text-brand-600 transition-colors">Home</RouterLink>
        <RouterLink
          to="/admin"
          class="px-4 py-2 bg-slate-900 text-white rounded-lg hover:bg-slate-800"
          >Admin</RouterLink
        >
      </div>
    </nav>
  </header>

  <main class="max-w-4xl mx-auto mt-10 p-4">
    <RouterView />
  </main>
</template>
