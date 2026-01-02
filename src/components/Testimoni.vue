<template>
  <div class="container my-5" id="testimoni">
    <!-- Heading -->
    <div class="text-center py-5">
      <h1 class="text-primary">Testimoni Klien</h1>
      <p class="text-muted">
        Beberapa Testimoni Pelanggan yang sudah menerima jasa kami
      </p>
    </div>

    <!-- Swiper Marquee -->
    <Swiper
      :modules="[Autoplay]"
      :loop="true"
      :slides-per-view="'auto'"
      :space-between="24"
      :speed="15000"
      :autoplay="{
        delay: 0,
        disableOnInteraction: false,
        reverseDirection: true,
      }"
      :allow-touch-move="false"
      class="portfolio-swiper"
    >
      <!-- Duplicate slide otomatis 2x agar loop mulus -->
      <SwiperSlide
        v-for="(img, index) in duplicatedImages"
        :key="index"
        class="swiper-slide-custom"
      >
        <img :src="img" alt="portfolio" />
      </SwiperSlide>
    </Swiper>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";
import "swiper/css";

import Testimoni1 from "../assets/testimoni/testimoni1.png";
import Testimoni2 from "../assets/testimoni/testimoni2.png";
import Testimoni3 from "../assets/testimoni/testimoni3.png";
import Testimoni4 from "../assets/testimoni/testimoni4.png";
import Testimoni5 from "../assets/testimoni/testimoni5.png";

// Array asli gambar
const images = [Testimoni1, Testimoni2, Testimoni3, Testimoni4, Testimoni5];

// Duplikasi otomatis 2x agar loop mulus
const duplicatedImages = [...images, ...images];
</script>

<style scoped>
.portfolio-swiper {
  overflow: hidden;
}

.swiper-slide-custom {
  width: 260px !important;
}

.swiper-slide-custom img {
  width: 100%;
  border-radius: 12px;
}
</style>
