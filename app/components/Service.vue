<script setup lang="ts">
import ServiceCard from "./ServiceCard.vue";
</script>

<template>
  <div class="px-60 py-20 bg-gray-100 w-full">
    <div class="text-center">
      <h2 class="text-4xl">Layanan Kami</h2>
      <p class="leading-loose my-10">
        Ady Trans Jaya menyediakan jasa pengiriman barang, sewa kendaraan, serta
        kontrak kendaraan untuk mendukung kebutuhan distribusi dan operasional
        bisnis Anda. Dengan armada yang terawat dan layanan yang fleksibel, kami
        siap menjadi solusi transportasi yang aman, tepat waktu, dan terpercaya.
      </p>
    </div>
    <div class="space-y-3">
      <ServiceCard
        src="/service1.jpg"
        alt="service 1"
        title="Jasa Pengiriman"
        description="Layanan pengiriman barang yang cepat, aman, dan tepat waktu untuk kebutuhan bisnis maupun personal, dengan armada terawat dan pengemudi berpengalaman."
      />
      <ServiceCard
        src="/service2.jpg"
        alt="service 2"
        title="Sewa Kendaraan"
        description="Layanan sewa kendaraan fleksibel untuk kebutuhan harian, mingguan, maupun bulanan, cocok untuk operasional usaha, distribusi, dan kegiatan logistik Anda."
      />
      <ServiceCard
        src="/service3.jpg"
        alt="service 3"
        title="Kontrak Kendaraan"
        description="Layanan sewa kendaraan fleksibel untuk kebutuhan harian, mingguan, maupun bulanan, cocok untuk operasional usaha, distribusi, dan kegiatan logistik Anda."
      />
    </div>
  </div>
</template>
