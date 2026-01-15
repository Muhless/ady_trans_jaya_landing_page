<script setup lang="ts">
defineProps<{
  label: string;
  id: string;
}>();
</script>

<template>
  <h2
    class="cursor-pointer text-white/80 hover:text-white transition-colors duration-200"
    :id="id"
  >
    {{ label }}
  </h2>
</template>
