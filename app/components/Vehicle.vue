<script setup lang="ts">
import { Autoplay, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import VehicleCard from "./VehicleCard.vue";

const modules = [Autoplay, Pagination];
</script>

<template>
  <div class="px-60 py-20 w-full">
    <div class="text-center w-full">
      <h2 class="text-4xl">Armada yang tepat untuk pengirimanmu</h2>
    </div>
    <div class="my-10">
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
            description="Mobil Pick Up berjenis Bak dengan ukuran 2 x 1,6 x 1,2 meter. Mobil ini
        cocok digunakan untuk mengangkut barang yang tidak memerlukan terlalu
        banyak tempat. Seperti sayur, buah-buahan, pasir, batu dan lain-lain."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/CDE.png"
            alt="mobil CDE"
            title="CDE"
            description="Colt Diesel Engkel (CDE), Mobil Box yang relatif kecil, memiliki ukuran kapasitas sebesar 2.2 x 1.35 x 1.3 meter. Cocok digunakan untuk mengirim barang di jalanan komplek perumahan atau gang-gang yang hanya bisa dilalui oleh kendaraan roda dua dan mobil biasa."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/CDD.png"
            alt="mobil CDD"
            title="CDD"
            description="Truk Colt Diesel Double (CDD), Mobil Box yang memiliki kapasitas lebih besar dari mobil box CDE, yaitu sebesar 4.5 x 2 x 2 meter. Mobil ini cocok digunakan untuk mengirim barang dengan jumlah yang banyak."
          />
        </SwiperSlide>

        <SwiperSlide>
          <VehicleCard
            src="/vehicles/fuso.png"
            alt="mobil fuso box"
            title="Fuso Box"
            description="Mobil Fuso bertype Box yang memiliki kapasitas sangat besar yaitu 5,7 x 2,5 x 2,5 meter. Mobil ini mampu mengangkut beban hingga 8000 kg, sehingga mobil ini cocok digunakan untuk mengangkut berbagai jenis barang yang besar dan berat, seperti plat besi, baja, kayu, kabel, beras, pupuk, hingga alat-alat proyek lainnya."
          />
        </SwiperSlide>
      </Swiper>
    </div>
  </div>
</template>
