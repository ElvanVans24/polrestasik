<template>
 <div id="carouselExampleCaptions" class="carousel slide bg-dark" data-bs-ride="carousel">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
      aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
      aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
      aria-label="Slide 3"></button>
  </div>

  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="/img/mako.jpg" class="d-block w-100 img-fluid" alt="Slide 1" style="max-height: 70vh; object-fit: cover;">
      <div class="carousel-caption d-none d-md-block">
        <h5 class="bg-dark bg-opacity-50 p-2 rounded">Polres Tasikmalaya Kota</h5>
      </div>
    </div>

    <div class="carousel-item">
      <img src="/img/header.png" class="d-block w-100 img-fluid" alt="Slide 2" style="max-height: 70vh; object-fit: cover;">
      <div class="carousel-caption d-none d-md-block">
        <h5 class="bg-dark bg-opacity-50 p-2 rounded">Header Slide</h5>
      </div>
    </div>

    <div class="carousel-item">
      <img src="/img/polri.jpg" class="d-block w-100 img-fluid" alt="Slide 3" style="max-height: 70vh; object-fit: cover;">
      <div class="carousel-caption d-none d-md-block">
        <h5 class="bg-dark bg-opacity-50 p-2 rounded">Polri Slide</h5>
      </div>
    </div>
  </div>

  <!-- Controls -->
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>


  <!-- Bagian Sejarah -->
  <div class="container-fluid bg-black bg-opacity-50 py-3">
      <div class="container">
        <div class="row py-2">
          <div class="col-12">
            <h1 class="text-warning text-center mb-1 sejarah_title">SEJARAH POLRES TASIKMALAYA KOTA</h1>
            <p class="fs-5 mb-5 pt-3 sejarah_text">
              Polres Tasikmalaya Kota merupakan salah satu instansi kepolisian yang beroperasi di Kota Tasikmalaya, Jawa Barat.
              Saat ini, Kapolres Tasikmalaya Kota adalah <strong>AKBP Moh. Faruk Rozi, S.H., S.I.K., M.Si.</strong>.
              Kota Tasikmalaya dijuluki sebagai <em>"Sang Mutiara dari Priangan Timur"</em> dan dikenal juga sebagai Kota Santri,
              terutama sebelum tahun 1980-an. Nama Tasikmalaya dipercaya berasal dari kata "danau yang bertebaran" atau
              "dauan di gugusan bukit".
              Dalam bahasa Sunda, Tasikmalaya juga diartikan sebagai "Keusik ngalayah", mengacu pada banyaknya pasir yang
              tersebar di area tersebut.
              Pada masa awal, wilayah ini dikenal dengan nama Sukapura, sebelumnya juga disebut Tawang atau Galunggung,
              yang merujuk pada Kerajaan Galunggung yang pernah berkuasa di wilayah tersebut.
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Tri Brata & Catur Prasetya -->
    <div class="container">
      <div class="row align-items-center py-5">
        <div class="col-md-4 text-center">
          <img src="/img/kapolres.png" class="img-fluid w-50 rounded-5 mb-4 tribrata_img" alt="Kapolres">
        </div>
        <div class="col-md-8 px-5 tribrata_text">
          <div class="mb-4">
            <h3 class="text-warning">TRI BRATA</h3>
            <ul class="fs-5">
              <li>Berbakti kepada nusa dan bangsa dengan penuh ketakwaan terhadap Tuhan Yang Maha Esa.</li>
              <li>Menjunjung tinggi kebenaran, keadilan, dan kemanusiaan dalam menegakkan hukum Negara Kesatuan Republik Indonesia.</li>
              <li>Senantiasa melindungi, mengayomi, dan melayani masyarakat dengan keikhlasan untuk mewujudkan keamanan dan ketertiban.</li>
            </ul>
          </div>
          <div>
            <h3 class="text-warning">CATUR PRASETYA</h3>
            <ul class="fs-5">
              <li>Meniadakan segala bentuk gangguan keamanan.</li>
              <li>Menjaga keselamatan jiwa, raga, harta benda, dan hak asasi manusia.</li>
              <li>Menjamin kepastian berdasarkan hukum.</li>
              <li>Memelihara perasaan tentram dan damai.</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
</template>


<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'

onMounted(() => {
  // Animate sejarah title
  gsap.from('.sejarah_title', {
    opacity: 0,
    y: 100,
    duration: 1,
    ease: 'power2.out'
  })

  // Animate sejarah text
  gsap.from('.sejarah_text', {
    opacity: 0,
    y: 50,
    duration: 1,
    ease: 'power3.out',
    delay: 0.3
  })

  // Animate tribrata image
  gsap.from('.tribrata_img', {
    opacity: 0,
    x: -100,
    duration: 1,
    ease: 'power3.out',
    delay: 0.5
  })

  // Animate tribrata text
  gsap.from('.tribrata_text', {
    opacity: 0,
    x: 100,
    duration: 1,
    ease: 'power3.out',
    delay: 0.7
  })
})
</script>

<style scoped>
/* Ensure image responsiveness */
.tribrata_img {
  max-width: 100%;
}
</style>