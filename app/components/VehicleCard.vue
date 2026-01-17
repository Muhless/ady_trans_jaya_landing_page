<template>
  <div
    class="bg-gray-100 rounded-2xl py-10 px-6 md:px-10 lg:px-20 grid grid-cols-1 md:grid-cols-2 gap-10 items-center"
  >
    <!-- Text -->
    <div>
      <h2 class="text-xl md:text-2xl font-bold mb-4">
        {{ title }}
      </h2>

      <p class="leading-relaxed md:leading-loose text-gray-700">
        {{ description }}
      </p>
    </div>

    <!-- Image -->
    <div class="w-full h-60 sm:h-72 md:h-80">
      <img
        :src="src"
        :alt="alt"
        class="w-full h-full object-cover rounded-xl"
      />
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
