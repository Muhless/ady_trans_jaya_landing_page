<script setup lang="ts">
defineProps<{
  label: string;
}>();
</script>

<template>
  <h2 class="cursor-pointer text-white/80  hover:text-white">{{ label }}</h2>
</template>
