<template>
  <div
    class="bg-white rounded-2xl overflow-hidden shadow-sm hover:shadow-lg transition"
  >
    <!-- Image -->
    <div class="w-full h-52 sm:h-60 md:h-64">
      <img :src="src" :alt="alt" class="w-full h-full object-cover" />
    </div>

    <!-- Content -->
    <div class="p-6 text-center sm:text-left">
      <h3 class="text-xl font-bold mb-3">
        {{ title }}
      </h3>

      <p class="text-gray-600 leading-relaxed text-sm md:text-base">
        {{ description }}
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  src: string;
  alt: string;
  title: string;
  description: string;
}>();
</script>
