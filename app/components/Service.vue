<script setup lang="ts">
import ServiceCard from "./ServiceCard.vue";
</script>

<template>
  <section id="services" class="w-full bg-gray-100 py-16 md:py-24">
    <div class="max-w-7xl mx-auto px-6 md:px-10">
      <!-- Title -->
      <div class="text-center max-w-3xl mx-auto mb-12">
        <h2 class="text-3xl md:text-4xl font-bold">Layanan Kami</h2>

        <p class="mt-6 text-gray-600 leading-relaxed text-base md:text-lg">
          Ady Trans Jaya menyediakan jasa pengiriman barang, sewa kendaraan,
          serta kontrak kendaraan untuk mendukung kebutuhan distribusi dan
          operasional bisnis Anda. Dengan armada terawat dan layanan fleksibel,
          kami siap menjadi solusi transportasi yang aman, tepat waktu, dan
          terpercaya.
        </p>
      </div>

      <!-- Cards -->
      <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-8">
        <ServiceCard
          src="/service1.jpg"
          alt="service 1"
          title="Jasa Pengiriman"
          description="Layanan pengiriman barang yang cepat, aman, dan tepat waktu untuk kebutuhan bisnis maupun personal."
        />

        <ServiceCard
          src="/service2.jpg"
          alt="service 2"
          title="Sewa Kendaraan"
          description="Sewa kendaraan harian, mingguan, hingga bulanan sesuai kebutuhan operasional Anda."
        />

        <ServiceCard
          src="/service3.jpg"
          alt="service 3"
          title="Kontrak Kendaraan"
          description="Solusi kontrak kendaraan jangka panjang untuk mendukung distribusi bisnis yang stabil."
        />
      </div>
    </div>
  </section>
</template>
