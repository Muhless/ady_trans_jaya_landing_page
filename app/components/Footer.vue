<template>
  <footer class="bg-black text-white pt-16 pb-6">
    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-5 gap-10 px-6">
      <div>
        <img src="/logo2.png" class="h-24 mb-4" />
        <p class="text-white/70 text-sm leading-relaxed">
          PT. Ady Trans Jaya adalah perusahaan jasa pengiriman dan transportasi
          terpercaya dengan layanan sewa dan kontrak kendaraan.
        </p>
      </div>

      <div>
        <h3 class="font-semibold mb-4">Menu</h3>
        <ul class="space-y-2 text-white/70">
          <li><a href="#about">Tentang Kami</a></li>
          <li><a href="#services">Layanan</a></li>
          <li><a href="#vehicles">Armada</a></li>
          <li><a href="#contact">Kontak</a></li>
        </ul>
      </div>

      <!-- Layanan -->
      <div>
        <h3 class="font-semibold mb-4">Layanan</h3>
        <ul class="space-y-2 text-white/70">
          <li>Jasa Pengiriman</li>
          <li>Sewa Kendaraan</li>
          <li>Kontrak Kendaraan</li>
        </ul>
      </div>

      <!-- Kontak -->
      <div>
        <h3 class="font-semibold mb-4">Kontak</h3>
        <ul class="space-y-2 text-white/70 text-sm">
          <li>Tangerang, Banten</li>
          <li>0838-7973-5470</li>
          <li>adytransjaya@gmail.com</li>
        </ul>
      </div>

      <div class="w-full h-32 md:h-48 rounded-xl overflow-hidden">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3965.7373979151744!2d106.38026617510535!3d-6.298197961641522!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e4205004485af25%3A0xa35984220006d65e!2sAdi%20Trans%20Jaya!5e0!3m2!1sid!2sid!4v1768637140218!5m2!1sid!2sid"
          class="w-full h-full border-0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </div>

    <div class="text-center text-white text-sm border-t border-white/10 pt-4">
      © {{ year }} PT. Ady Trans Jaya. All rights reserved.
    </div>
  </footer>
</template>

<script setup>
const year = new Date().getFullYear();
</script>
