<script setup>
import gsap from "gsap";
import { onMounted } from "vue";
import Topbar from "./topbar/index.vue";

onMounted(() => {
  gsap.from("h1", {
    y: 30,
    opacity: 0,
    duration: 1,
    ease: "power2.out",
  });
});
</script>

<template>
  <div class="relative w-full h-[780px]">
    <img
      src="/hero.jpg"
      alt="Jasa Pengiriman Ady Trans Jaya"
      class="w-full h-full object-cover"
    />
    <div class="absolute inset-0 bg-black/40"></div>
    <div class="absolute inset-0 z-10">
      <Topbar />
    </div>
    <div
      class="absolute inset-0 z-10 flex flex-col items-center mt-48 text-white"
    >
      <h1 class="text-7xl font-bold">Kirim Lebih Cepat</h1>
      <h2 class="text-4xl">
        Dengan <span class="hover:text-sky-500 font-bold">Ady Trans Jaya</span>
      </h2>
    </div>
  </div>
</template>
