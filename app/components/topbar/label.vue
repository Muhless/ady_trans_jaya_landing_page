<script setup lang="ts">
const emit = defineEmits(["click"]);

defineProps<{
  label: string;
  id: string;
}>();

const scrollToSection = (id: string) => {
  const element = document.getElementById(id);
  if (!element) return;

  const headerOffset = 64;
  const elementPosition = element.getBoundingClientRect().top;
  const offsetPosition = elementPosition + window.pageYOffset - headerOffset;

  window.scrollTo({
    top: offsetPosition,
    behavior: "smooth",
  });

  emit("click"); // 🔥 penting
};
</script>

<template>
  <button
    @click="scrollToSection(id)"
    class="cursor-pointer text-white/80 hover:text-white transition text-base py-2"
  >
    {{ label }}
  </button>
</template>
