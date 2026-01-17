<script setup lang="ts">
import { onMounted, onUnmounted, ref } from "vue";
import Label from "./label.vue";

const isScrolled = ref(false);
const isOpen = ref(false);

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50;
};

const scrollToTop = () => {
  window.scrollTo({ top: 0, behavior: "smooth" });
  isOpen.value = false;
};

const toggleMenu = () => {
  isOpen.value = !isOpen.value;
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<template>
  <header
    :class="[
      'w-full h-16 sticky top-0 z-50 transition-all duration-300',
      isScrolled ? 'bg-black shadow-lg' : 'bg-black/30 backdrop-blur',
    ]"
  >
    <div
      class="max-w-7xl mx-auto h-full px-6 flex items-center justify-between"
    >
      <!-- Logo -->
      <img
        src="/logo2.png"
        alt="Ady Trans Jaya"
        class="h-12 sm:h-14 cursor-pointer"
        @click="scrollToTop"
      />

      <!-- Desktop Menu -->
      <nav class="hidden md:flex items-center gap-8 text-sm">
        <Label label="Tentang Kami" id="abouts" />
        <Label label="Layanan" id="services" />
        <Label label="Armada" id="vehicles" />
        <Label label="Kontak" id="contacts" />
      </nav>

      <!-- Mobile Button -->
      <button
        @click="toggleMenu"
        class="md:hidden text-white text-3xl focus:outline-none"
      >
        ☰
      </button>
    </div>

    <!-- Mobile Menu -->
    <div
      v-show="isOpen"
      class="md:hidden bg-black/95 backdrop-blur border-t border-white/10"
    >
      <div class="flex flex-col text-center py-6 space-y-4">
        <Label label="Tentang Kami" id="abouts" @click="isOpen = false" />
        <Label label="Layanan" id="services" @click="isOpen = false" />
        <Label label="Armada" id="vehicles" @click="isOpen = false" />
        <Label label="Kontak" id="contacts" @click="isOpen = false" />
      </div>
    </div>
  </header>
</template>
