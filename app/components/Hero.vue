<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <div class="relative w-full h-screen">
    <img
      src="/hero.jpg"
      alt="Jasa Pengiriman Ady Trans Jaya"
      class="absolute inset-0 w-full h-full object-cover"
    />

    <div class="absolute inset-0 bg-black/40 pointer-events-none"></div>

    <div class="absolute top-0 left-0 w-full z-30">
      <Topbar />
    </div>

    <div
      class="absolute inset-0 flex flex-col items-center justify-center text-white text-center pointer-events-none"
    >
      <h1 class="text-7xl font-bold">Kirim Lebih Cepat</h1>
      <h2 class="text-4xl mt-3">
        Dengan
        <span class="hover:text-sky-500 font-bold"> Ady Trans Jaya </span>
      </h2>
      <a
        href="https://wa.me/6283813343637"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Hubungi Ady Trans Jaya via WhatsApp"
        class="mt-10 bg-sky-500 py-2 px-14 rounded-md flex items-center gap-3 hover:bg-sky-700 transition-colors duration-200 pointer-events-auto"
      >
        <span class="text-lg font-medium">Hubungi Kami</span>
        <Icon icon="mdi:whatsapp" class="text-2xl" />
      </a>
    </div>
  </div>
</template>
