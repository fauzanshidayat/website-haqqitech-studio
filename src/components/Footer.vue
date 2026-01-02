<template>
  <footer class="bg-light text-light pt-5">
    <div class="container" id="kontak">
      <!-- Row Utama: 3 Column -->
      <div class="row">
        <!-- Column Kiri: Link Terkait -->
        <div class="col-md-4 mb-4">
          <h5 class="text-primary">Link Terkait</h5>
          <ul class="list-unstyled">
            <li>
              <a href="/" class="text-black text-decoration-none">Home</a>
            </li>
            <li>
              <a href="#layanan" class="text-black text-decoration-none"
                >Layanan</a
              >
            </li>
            <li>
              <a href="#portfolio" class="text-black text-decoration-none"
                >Portfolio</a
              >
            </li>
            <li>
              <a href="#testimoni" class="text-black text-decoration-none"
                >Testimoni</a
              >
            </li>
            <li>
              <a href="#kontak" class="text-black text-decoration-none"
                >Kontak</a
              >
            </li>
          </ul>
        </div>

        <!-- Column Tengah: Kontak -->
        <div class="col-md-4 mb-4">
          <h5 class="text-primary">Kontak Kami</h5>
          <p class="mb-1 text-black">
            <strong>Telepon:</strong> 0838-9915-1073
          </p>
          <p class="mb-1 text-black">
            <strong>Telepon:</strong> 0852-1587-2297
          </p>
          <p class="mb-1 text-black">
            <strong>Email:</strong> haqqitechstudio@gmail.com
          </p>
          <p class="mb-1 text-black">
            <strong>Alamat:</strong> Des. Bantar Panjang, Kec. Cikesual, Kab.
            Serang - Prov. Banten
          </p>
        </div>

        <!-- Column Kanan: Google Maps -->
        <div class="col-md-4 mb-4">
          <h5 class="text-primary">Lokasi</h5>
          <div class="ratio ratio-16x9">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.2671794246844!2d106.25821317409644!3d-6.228463260995895!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e421db4201c5cf3%3A0xeb60f91680cb614!2sSDN%20Bantar%20Panjang!5e0!3m2!1sid!2sid!4v1767365698548!5m2!1sid!2sid"
              width="600"
              height="450"
              style="border: 0"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
            ></iframe>
          </div>
        </div>
      </div>
      <hr class="text-black" />
      <!-- Row Bawah: Copyright -->
      <div class="row py-3">
        <div class="col text-center text-black">
          <p>&copy; 2025 HaqqiTech Studio. All Rights Reserved.</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  font-family: Arial, sans-serif;
}

footer h5 {
  font-weight: 600;
  margin-bottom: 1rem;
}

footer a:hover {
  text-decoration: underline;
}
</style>
