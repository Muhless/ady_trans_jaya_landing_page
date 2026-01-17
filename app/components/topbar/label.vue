<script setup lang="ts">
defineProps<{
  label: string;
  id: string;
}>();

const scrollToSection = (id: string) => {
  const element = document.getElementById(id);
  if (element) {
    const headerOffset = 64; // h-16 = 64px
    const elementPosition = element.getBoundingClientRect().top;
    const offsetPosition = elementPosition + window.pageYOffset - headerOffset;

    window.scrollTo({
      top: offsetPosition,
      behavior: "smooth",
    });
  }
};
</script>

<template>
  <button
    @click="scrollToSection(id)"
    class="cursor-pointer text-white/80 hover:text-white transition"
  >
    {{ label }}
  </button>
</template>
