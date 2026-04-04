<script setup>
import Desain from "../assets/desaign.png";
import LandingPage from "../assets/landingpage.png";
import Webapp from "../assets/webapp.png";
</script>

<template>
  <div class="container" id="layanan">
    <!-- Judul Section -->
    <div class="text-center py-5">
      <h1 class="text-primary">Layanan Kami</h1>
      <p class="text-muted">
        Kami menyediakan layanan profesional untuk kebutuhan Anda
      </p>
    </div>

    <!-- Row Card -->
    <div class="row g-4">
      <!-- Card 1 -->
      <div class="col-md-4">
        <div class="card h-100">
          <img :src="Desain" class="card-img-top" alt="Desain Website" />
          <div class="card-body text-center">
            <h5 class="card-title">Desaign Kaligrafi</h5>
            <p class="card-text">
              Desain kaligrafi yang indah dan berkarakter, cocok untuk
              pesantren, UMKM,kebutuhan pribadi, dan lainnya. Bisa untuk tulisan
              arab, quote islami, atau dekorasi dan lain lain.
            </p>
            <a href="https://wa.link/dlru5x" target="_blank"
              ><button type="button" class="btn btn-primary">
                Pesan Sekarang
              </button></a
            >
          </div>
        </div>
      </div>

      <!-- Card 2 -->
      <div class="col-md-4">
        <div class="card h-100">
          <img :src="Webapp" class="card-img-top" alt="Pengembangan Aplikasi" />
          <div class="card-body text-center">
            <h5 class="card-title">Web Aplikasi</h5>
            <p class="card-text">
              Pembuatan web aplikasi yang cepat, aman, dan sesuai kebutuhan.
              Cocok untuk bisnis, UMKM, Sekolah maupun sistem sederhana yang
              memudahkan aktivitas Anda.
            </p>
            <a href="https://wa.link/w2d1i5" target="_blank"
              ><button type="button" class="btn btn-primary">
                Pesan Sekarang
              </button></a
            >
          </div>
        </div>
      </div>

      <!-- Card 3 -->
      <div class="col-md-4">
        <div class="card h-100">
          <img
            :src="LandingPage"
            class="card-img-top"
            alt="Digital Marketing"
          />
          <div class="card-body text-center">
            <h5 class="card-title">Landing Page</h5>
            <p class="card-text">
              Desain landing page yang menarik, responsif, dan mudah dipahami.
              Cocok untuk promosi produk, jasa, atau kebutuhan bisnis biar
              tampil lebih profesional dan meyakinkan.
            </p>
            <a href="https://wa.link/w2d1i5" target="_blank"
              ><button type="button" class="btn btn-primary">
                Pesan Sekarang
              </button></a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
