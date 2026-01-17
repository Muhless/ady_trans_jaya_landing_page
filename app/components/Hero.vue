<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <div class="relative w-full h-screen -mt-16">
    <!-- Background -->
    <img
      src="/hero.jpg"
      alt="Jasa Pengiriman Ady Trans Jaya"
      class="absolute inset-0 w-full h-full object-cover"
    />

    <!-- Overlay -->
    <div class="absolute inset-0 bg-black/40 pointer-events-none"></div>

    <!-- Content -->
    <div
      class="absolute inset-0 flex flex-col items-center justify-center text-white text-center px-6"
    >
      <h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold">
        Kirim Lebih Cepat
      </h1>

      <h2 class="mt-3 text-xl sm:text-2xl md:text-3xl lg:text-4xl">
        Dengan
        <span class="text-sky-400 font-bold"> Ady Trans Jaya </span>
      </h2>

      <!-- CTA -->
      <a
        href="https://wa.me/6283813343637"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Hubungi Ady Trans Jaya via WhatsApp"
        class="mt-10 bg-sky-500 py-3 px-14 rounded-md flex items-center gap-3 hover:bg-sky-700 transition-colors duration-200"
      >
        <span class="text-lg font-medium">Hubungi Kami</span>
        <Icon icon="mdi:whatsapp" class="text-2xl" />
      </a>
    </div>
  </div>
</template>
