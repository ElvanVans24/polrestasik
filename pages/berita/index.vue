<template>
  <div class="container my-5">
    <h1 class="text-center mb-5 berita_title">BERITA TERBARU</h1>
    <div class="card-group pt-3 pb-3 berita_cards">
      <div class="card shadow p-3 mb-5 bg-body-tertiary mx-1 rounded">
        <img src="/img/berita1.jpg" class="card-img-top" alt="Berita 1">
        <div class="card-body d-flex flex-column justify-content-between">
          <h6 class="card-title">POLRES TASIKMALAYA KOTA GELAR PEMUSNAHAN BARANG BUKTI HASIL OPERASI KRYD</h6>
          <div class="">
            <p class="card-text"><small class="text-body-secondary">Last updated 3 mins ago</small></p>
            <a href="/berita/srl" class="btn bg-warning bg-gradient">Selengkapnya</a>
          </div>
        </div>
      </div>
      <div class="card shadow p-3 mb-5 bg-body-tertiary mx-1 rounded">
        <img src="/img/berita2.jpg" class="card-img-top" alt="Berita 2">
        <div class="card-body d-flex flex-column justify-content-between">
          <h6 class="card-title">Polres Tasikmalaya Kota Gelar Apel Kesiapan Siagaan dan Apel Premanisme Bersama Forkopimda</h6>
          <div class="">
            <p class="card-text"><small class="text-body-secondary">Last updated 3 mins ago</small></p>
            <a href="/berita/zona" class="btn bg-warning bg-gradient">Selengkapnya</a>
          </div>
        </div>
      </div>
      <div class="card shadow p-3 mb-5 bg-body-tertiary mx-1 rounded">
        <img src="/img/berita3.jpg" class="card-img-top" alt="Berita 3">
        <div class="card-body d-flex flex-column justify-content-between">
          <h6 class="card-title">Polres Tasikmalaya Kota Gelar Apel Gabungan Kesiapan Siagaan untuk Operasi Ketupat Lodaya2025</h6>
          <div class="">
            <p class="card-text"><small class="text-body-secondary">Last updated 3 mins ago</small></p>
            <a href="/berita/sc2024" class="btn bg-warning bg-gradient">Selengkapnya</a>
          </div>
        </div>
      </div>
      <div class="card shadow p-3 mb-5 bg-body-tertiary mx-1 rounded">
        <img src="/img/berita4.jpg" class="card-img-top" alt="Berita 4">
        <div class="card-body d-flex flex-column justify-content-between">
          <h6 class="card-title">Kapolres Tasikmalaya Kota menerapkan rekayasa lalu lintas di Simpang Tiga Pamoyanan</h6>
          <div class="">
            <p class="card-text"><small class="text-body-secondary">Last updated 3 mins ago</small></p>
            <a href="/berita/us" class="btn bg-warning bg-gradient">Selengkapnya</a>
          </div>
        </div>
      </div>
      <div class="card shadow p-3 mb-5 bg-body-tertiary mx-1 rounded">
        <img src="/img/berita5.jpg" class="card-img-top" alt="Berita 5">
        <div class="card-body d-flex flex-column justify-content-between">
          <h6 class="card-title">Dalam rangka memastikan keamanan dan kelancaran arus mudik Lebaran, Kapolres Tasikmalaya Kota melakukan monitoring di Ampera Waterpark</h6>
          <div class="">
            <p class="card-text"><small class="text-body-secondary">Last updated 3 mins ago</small></p>
            <a href="/berita/upacara" class="btn bg-warning bg-gradient">Selengkapnya</a>
          </div>
        </div>
      </div>
    </div>
    <!-- Add more card groups as needed, truncated for brevity -->
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'

onMounted(() => {
  // Animate title
  gsap.from('.berita_title', {
    opacity: 0,
    y: 100,
    duration: 1,
    ease: 'power2.out'
  })

  // Animate cards
  gsap.from('.berita_cards .card', {
    opacity: 0,
    y: 50,
    duration: 0.8,
    ease: 'power3.out',
    stagger: 0.1,
    delay: 0.5
  })
})
</script>

<style scoped>
.card-img-top {
  height: 200px;
  object-fit: contain;
}
</style>