<template>
  <div class="w-full">
    <div class="grid grid-cols-2 rounded-2xl bg-white h-72">
      <div class="flex flex-col px-20 justify-center">
        <h2 class="text-2xl font-bold">{{ title }}</h2>
        <p class="leading-loose">{{ description }}</p>
      </div>
      <div class="h-72">
        <img
          :src="src"
          :alt="alt"
          class="w-full h-full object-cover rounded-r-2xl"
        />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
defineProps<{
  src: string;
  alt?: string;
  title: string;
  description: string;
}>();
</script>
