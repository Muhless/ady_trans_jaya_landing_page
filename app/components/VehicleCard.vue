<template>
  <div
    class="bg-gray-100 grid grid-cols-2 items-center px-20 justify-between rounded-2xl py-10"
  >
    <div class="">
      <h2 class="text-2xl font-bold">{{ title }}</h2>
      <p class="leading-loose">
        {{ description }}
      </p>
    </div>
    <div class="h-72 w-full items-center">
      <img :src="src" :alt="alt" class="w-full h-full object-cover" />
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
