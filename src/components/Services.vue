<script setup>
import Desain from "../assets/desaign.png";
import uiux from "../assets/uiux.png";
import Webdev from "../assets/webdev.png";
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
            <h5 class="card-title">Graphic Desaign</h5>
            <p class="card-text">
              Desain grafis modern yang menarik dan sesuai dengan identitas
              brand Anda. Cocok untuk branding, materi promosi, atau konten
              visual.
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
          <img :src="Webdev" class="card-img-top" alt="Pengembangan Aplikasi" />
          <div class="card-body text-center">
            <h5 class="card-title">Web Development</h5>
            <p class="card-text">
              Pembuatan website dan aplikasi web dengan performa tinggi, aman,
              dan sesuai kebutuhan bisnis Anda.
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
          <img :src="uiux" class="card-img-top" alt="Digital Marketing" />
          <div class="card-body text-center">
            <h5 class="card-title">UI/UX Desaign</h5>
            <p class="card-text">
              Desain interface aplikasi dan website yang responsif, intuitif,
              dan meningkatkan pengalaman pengguna.
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
