<script setup lang="ts">
import { Autoplay, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import VehicleCard from "./VehicleCard.vue";

const modules = [Autoplay, Pagination];
</script>

<template>
  <section class="w-full px-6 py-16 md:px-20 lg:px-40 xl:px-60">
    <!-- Title -->
    <div class="text-center">
      <h2 class="text-2xl md:text-3xl lg:text-4xl font-semibold">
        Armada yang tepat untuk pengirimanmu
      </h2>
    </div>

    <!-- Slider -->
    <div class="mt-10">
      <Swiper
        :modules="modules"
        :slides-per-view="1"
        :space-between="24"
        :loop="true"
        :autoplay="{ delay: 3000, disableOnInteraction: false }"
        :pagination="{ clickable: true }"
        class="w-full"
      >
        <SwiperSlide>
          <VehicleCard
            src="/vehicles/pickup.png"
            alt="mobil pickup"
            title="Pick Up"
            description="Mobil Pick Up berjenis bak dengan ukuran 2 x 1,6 x 1,2 meter. Cocok untuk pengangkutan barang ringan seperti sayur, buah, pasir, batu, dan kebutuhan distribusi lainnya."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/CDE.png"
            alt="mobil CDE"
            title="CDE"
            description="Colt Diesel Engkel (CDE) dengan kapasitas 2.2 x 1.35 x 1.3 meter. Ideal untuk area perumahan, jalan sempit, dan pengiriman dalam kota."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/CDD.png"
            alt="mobil CDD"
            title="CDD"
            description="Colt Diesel Double (CDD) berkapasitas 4.5 x 2 x 2 meter. Cocok untuk pengiriman barang dalam jumlah besar dan distribusi antar kota."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/fuso.png"
            alt="mobil fuso box"
            title="Fuso Box"
            description="Fuso Box berkapasitas besar 5.7 x 2.5 x 2.5 meter dengan daya angkut hingga 8 ton. Cocok untuk proyek besar, logistik industri, dan muatan berat."
          />
        </SwiperSlide>
      </Swiper>
    </div>
  </section>
</template>
