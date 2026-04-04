<template>
  <div class="bg-light">
    <div class="container my-5" id="portfolio">
      <!-- Heading -->
      <div class="text-center py-5">
        <h1 class="text-primary">Portfolio Kami</h1>
        <p class="text-muted">
          Beberapa karya terbaik kami yang telah berhasil kami kerjakan
        </p>
      </div>

      <!-- Swiper Marquee -->
      <Swiper
        :modules="[Autoplay]"
        :loop="true"
        :slides-per-view="'auto'"
        :space-between="24"
        :speed="15000"
        :autoplay="{ delay: 0, disableOnInteraction: false }"
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
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";
import "swiper/css";

import Karya1 from "../assets/portfolio/karya1.jpg";
import Karya2 from "../assets/portfolio/karya2.jpg";
import Karya3 from "../assets/portfolio/karya3.png";
import Karya4 from "../assets/portfolio/karya4.png";
import Karya5 from "../assets/portfolio/karya5.png";
import Karya6 from "../assets/portfolio/karya6.png";
import Karya7 from "../assets/portfolio/karya7.png";
import Karya8 from "../assets/portfolio/karya8.png";
import Karya9 from "../assets/portfolio/karya9.png";
import Karya10 from "../assets/portfolio/karya10.png";

// Array asli gambar
const images = [
  Karya1,
  Karya2,
  Karya3,
  Karya4,
  Karya5,
  Karya6,
  Karya7,
  Karya8,
  Karya9,
  Karya10,
];

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
