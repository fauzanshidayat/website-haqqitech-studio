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

      <!-- Swiper -->
      <div class="position-relative">
        <Swiper
          :modules="[Navigation]"
          :loop="true"
          :slides-per-view="'auto'"
          :space-between="24"
          :speed="600"
          :allow-touch-move="true"
          navigation
          class="portfolio-swiper"
        >
          <SwiperSlide
            v-for="(item, index) in duplicatedImages"
            :key="index"
            class="swiper-slide-custom"
          >
            <div class="card portfolio-card shadow-sm">
              <img :src="item.image" class="card-img-top" alt="portfolio" />

              <div class="card-body">
                <h5 class="card-title">{{ item.title }}</h5>
                <p class="card-text text-muted">
                  {{ item.description }}
                </p>

                <a
                  v-if="item.isExternal"
                  :href="item.link"
                  target="_blank"
                  class="btn btn-primary btn-sm w-100"
                >
                  Lihat Detail →
                </a>

                <router-link
                  v-else
                  :to="item.link"
                  class="btn btn-primary btn-sm w-100"
                >
                  Lihat Detail →
                </router-link>
              </div>
            </div>
          </SwiperSlide>
        </Swiper>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";
import "swiper/css";
import "swiper/css/navigation";

// Import gambar
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
import Karya11 from "../assets/portfolio/karya11.png";

const images = [
  {
    image: Karya1,
    title: "Khat Tsuluts Jali",
    description: "Khat Tsuluts Jali Klasik & Elegan.",
    link: "https://id.pinterest.com/pin/1139551511985809956/",
    isExternal: true,
  },
  {
    image: Karya2,
    title: "Khat Tsuluts Modern",
    description: "Khat Tsuluts Modern Simpel & Tegas.",
    link: "https://id.pinterest.com/pin/1139551511985811168/",
    isExternal: true,
  },
  {
    image: Karya3,
    title: "Khat Kufi Murabba’",
    description: "Khat Kufi Murabba’ Gaya Kotak-Kotak.",
    link: "https://id.pinterest.com/pin/1139551511985811167/",
    isExternal: true,
  },
  {
    image: Karya4,
    title: "Khat Diwani Jali",
    description: "Khat Diwani Jali Artistik & Padat.",
    link: "https://id.pinterest.com/pin/1139551511985811165/",
    isExternal: true,
  },
  {
    image: Karya5,
    title: "Khat Maghribi",
    description: "Khat Maghribi Ekspresi Bebas.",
    link: "https://id.pinterest.com/pin/1139551511985811169/",
    isExternal: true,
  },
  {
    image: Karya6,
    title: "Website Landing Page",
    description: "Website Landing Page HaqqiTech Studio",
    link: "https://haqqitechstudio.vercel.app/",
    isExternal: true,
  },
  {
    image: Karya7,
    title: "Website PSB",
    description: "Sistem Penerimaan Santri Baru PPM Nurul Alami.",
    link: "https://www.psb.nurulalami.sch.id/",
    isExternal: true,
  },
  {
    image: Karya8,
    title: "Website Simkes",
    description: "Sistem Informasi Monitoring Kegiatan Santri.",
    link: "https://www.simkes.nurulalami.sch.id/",
    isExternal: true,
  },
  {
    image: Karya9,
    title: "Website Resmi Nurul Alami",
    description: "Website Resmi PPM Nurul Alami.",
    link: "https://www.nurulalami.sch.id/",
    isExternal: true,
  },
  {
    image: Karya10,
    title: "Website Portfolio",
    description: "Website Portfolio Fauzan Hidayat",
    link: "https://fauzanhidayat.vercel.app/",
    isExternal: true,
  },
  {
    image: Karya11,
    title: "Website IKPPM NA",
    description: "Website Resmi IKPPM NA",
    link: "https://ikppm.nurulalami.sch.id/",
    isExternal: true,
  },
];

const duplicatedImages = [...images, ...images];
</script>

<style scoped>
.portfolio-swiper {
  overflow: hidden;
  padding: 10px 40px; /* biar tombol tidak nempel */
}

/* custom slide */
.swiper-slide-custom {
  width: 260px !important;
}

/* Card */
.portfolio-card {
  border-radius: 16px;
  overflow: hidden;
  transition: 0.3s;
}

.portfolio-card:hover {
  transform: translateY(-6px);
}

/* Image */
.portfolio-card img {
  height: 160px;
  object-fit: cover;
}

/* Text */
.card-title {
  font-size: 16px;
  font-weight: 600;
}

.card-text {
  font-size: 13px;
}

/* Button */
.btn {
  border-radius: 8px;
}

/* ===== NAVIGATION BUTTON STYLE ===== */
:deep(.swiper-button-next),
:deep(.swiper-button-prev) {
  color: #0d6efd;
  background: white;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
}

:deep(.swiper-button-next::after),
:deep(.swiper-button-prev::after) {
  font-size: 10px;
  font-weight: bold;
}
</style>
