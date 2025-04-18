<template>
  <div class="container my-5">
    <h1 class="text-center mb-5 prestasi_title">PRESTASI POLRES TASIKMALAYA KOTA</h1>
    <div class="row row-cols-1 row-cols-md-3 g-4 prestasi_cards">
      <div class="col">
        <div class="card">
          <img src="/img/srl.jpg" class="card-img-top" alt="Safety Riding">
          <div class="card-body">
            <h5 class="card-title">Pengujian Lintasan Safety Riding SMKN4 Tasikmalaya</h5>
            <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="/img/srl.jpg" class="card-img-top" alt="Safety Riding">
          <div class="card-body">
            <h5 class="card-title">Pengujian Lintasan Safety Riding SMKN4 Tasikmalaya</h5>
            <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="/img/srl.jpg" class="card-img-top" alt="Safety Riding">
          <div class="card-body">
            <h5 class="card-title">Pengujian Lintasan Safety Riding SMKN4 Tasikmalaya</h5>
            <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="/img/prestasi.jpg" class="card-img-top" alt="Prestasi">
          <div class="card-body">
            <h5 class="card-title">Prestasi Lainnya</h5>
            <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
          </div>
        </div>
      </div>
      <!-- Add more cards as needed, truncated for brevity -->
    </div>
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'

onMounted(() => {
  // Animate title
  gsap.from('.prestasi_title', {
    opacity: 0,
    y: 100,
    duration: 1,
    ease: 'power2.out'
  })

  // Animate cards
  gsap.from('.prestasi_cards .card', {
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
  object-fit: cover;
}
</style>