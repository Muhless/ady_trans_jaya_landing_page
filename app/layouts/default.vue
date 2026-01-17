<script setup lang="ts"></script>

<template>
  <div class="min-h-screen">
    <div class="fixed top-0 left-0 w-full z-50">
      <Topbar />
    </div>
    <main class="pt-16">
      <slot />
    </main>
  </div>
</template>
