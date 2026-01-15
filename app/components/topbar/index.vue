<script setup lang="ts">
import Label from "./label.vue";
</script>

<template>
  <header class="w-full h-16 bg-black/20">
    <div
      class="max-w-7xl mx-auto h-full px-6 flex items-center gap-3 justify-evenly"
    >
      <img src="/logo.png" alt="Logo Ady Trans Jaya" class="h-20 w-auto" />
      <Label label="Tentang Kami" id="about" />
      <Label label="Layanan Kami" id="services" />
      <Label label="Hubungi Kami" id="contact" />
    </div>
  </header>
</template>
