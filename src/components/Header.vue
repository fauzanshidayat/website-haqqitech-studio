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
            Haqqitech Studio siap membantu Anda menghadirkan solusi digital
            lengkap! Kami menyediakan layanan UI/UX, Desain Grafis, dan Web
            Development, cocok untuk branding, website, aplikasi, konten visual,
            dan kebutuhan digital lainnya.
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
