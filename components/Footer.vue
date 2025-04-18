<template>
  <footer class="bg-black bg-gradient text-white py-4">
    <div class="container">
      <div class="row gy-4">
        <!-- Hubungi Kami -->
        <div class="col-md-4 col-12">
          <div class="logo-container mb-2">
            <img src="/img/polda.png" alt="Logo Polda" class="img-fluid" style="max-width: 70px;">
          </div>
          <h5>Hubungi Kami</h5>
          <p>POLRES TASIKMALAYA KOTA.</p>
          <p>Jalan Letnan Harun No. 76 Tasikmalaya, Tasikmalaya, Indonesia, West Java</p>
          <p>
            <i class="fas fa-phone-alt"></i> No. HP Tim Maung Galunggung :<br />
            <i class="fas fa-phone-alt"></i> 0853-3555-6262<br />
            <i class="fas fa-phone-alt"></i> 0853-3555-6263<br />
            <i class="fas fa-envelope"></i>
            <a href="https://taplink.cc/polrestasikmalayakota" class="text-white d-block text-break">
              https://taplink.cc/polrestasikmalayakota
            </a>
          </p>
        </div>

        <!-- Media Sosial -->
        <div class="col-md-4 col-12">
          <div class="logo-container mb-2">
            <img src="/img/humaslogo.png" alt="Logo Humas" class="img-fluid" style="max-width: 90px;">
          </div>
          <h5>Media Sosial</h5>
          <ul class="list-unstyled">
            <li><a href="https://www.facebook.com/humas.polrestsmkota" class="text-white">Facebook</a></li>
            <li><a href="#" class="text-white">@PolresTasikKota (Twitter)</a></li>
            <li><a href="https://www.instagram.com/polrestasikkota/" class="text-white">Instagram</a></li>
          </ul>
        </div>

        <!-- Maps -->
        <div class="col-md-4 col-12">
          <h5>Maps Polres Tasikmalaya Kota</h5>
          <div class="ratio ratio-4x3 rounded-4 shadow overflow-hidden">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2962.903291788812!2d108.19294907346342!3d-7.307951671845943!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f574892269129%3A0x9f2e9331725cda02!2sPolres%20Tasikmalaya%20Kota!5e1!3m2!1sid!2sid!4v1744299512129!5m2!1sid!2sid"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
              style="border:0;">
            </iframe>
          </div>
        </div>
      </div>
    </div>

    <!-- Copyright -->
    <div class="text-center mt-4 small">
      <p class="mb-1">© HumasPolresTasikmalayaKota. All rights reserved.</p>
      <p>BY ELVAN MUHAMMAD FAUZAN <span class="text-primary">Operator</span></p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
footer {
  font-size: 0.9rem;
}
</style>
