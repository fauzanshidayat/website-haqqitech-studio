<script setup>
import Logo from "../assets/logo.png";
</script>
<template>
  <nav class="navbar navbar-expand-lg bg-white">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img :src="Logo" alt="Bootstrap" width="100%" height="50" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto fs-5">
          <li class="nav-item">
            <a class="nav-link text-black" aria-current="page" href="/">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-black" href="#layanan">Layanan</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-black" href="#portfolio">Portfolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-black" href="#testimoni">Testimoni</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-black" href="#kontak">Kontak</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
