<script setup>
import Hero from "../assets/hero.png";
</script>

<template>
  <div class="bg-light">
    <div class="container py-5">
      <div class="row align-items-center">
        <!-- Kolom kiri (Teks) -->
        <div class="col-md-6">
          <h1 class="text-primary">Butuh Layanan Digital Profesional ?</h1>
          <p>
            Haqqitech Studio siap membantu Anda menghadirkan solusi digital !
            Mulai dari desain kaligrafi, landing page, hingga web aplikasi,
            cocok untuk pesantren, Sekolah, UMKM, Bisnis, maupun kebutuhan
            pribadi. Bikin tampilan lebih menarik, rapi, dan berkesan.
          </p>
          <a href="#layanan"
            ><button class="btn btn-primary">Lihat Layanan</button></a
          >
        </div>

        <!-- Kolom kanan (Gambar) -->
        <div class="col-md-6 text-center">
          <img :src="Hero" class="img-fluid" alt="Gambar Contoh" />
        </div>
      </div>
    </div>
  </div>
</template>
