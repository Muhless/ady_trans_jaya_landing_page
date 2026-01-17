<script setup lang="ts">
import { onMounted, onUnmounted, ref } from "vue";
import Label from "./label.vue";

const isScrolled = ref(false);

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50; // Ubah warna setelah scroll 50px
};

const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: "smooth",
  });
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
      isScrolled ? 'bg-black shadow-lg' : 'bg-black/20 backdrop-blur-sm',
    ]"
  >
    <div
      class="max-w-7xl mx-auto h-full px-6 flex items-center gap-3 justify-evenly"
    >
      <img
        @click="scrollToTop"
        src="/logo2.png"
        alt="Logo Ady Trans Jaya"
        class="h-20 w-auto cursor-pointer"
      />
      <Label label="Tentang Kami" id="abouts" />
      <Label label="Layanan Kami" id="services" />
      <Label label="Armada Kami" id="vehicles" />
      <Label label="Hubungi Kami" id="contacts" />
    </div>
  </header>
</template>
