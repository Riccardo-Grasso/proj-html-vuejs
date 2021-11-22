<template>
  <header>
    <div class="container">
      <!-- Navbar contiene logo e icone -->
      <Navbar></Navbar>
      <!-- SEZIONE BARBER-SHOP -->
      <section class="hero-section row row-cols-2">
        <div class="col left-text d-flex">
          <h1 class="main-title section-title mb-4">Barber Shop</h1>
          <div class="line mb-4"></div>
          <p class="text mb-4">The Pinnacle of Male Grooming</p>
          <a class="proj-link" href="#">LEARN MORE</a>
        </div>
        <div class="col right-img">
          <img src="../assets/header-hero.png" alt="img" class="w-100" />
        </div>
      </section>
    </div>
  </header>
</template>

<script>
import Navbar from "../components/Navbar.vue";
export default {
  name: "Header",
  components: { Navbar },
  data() {
    return {};
  },
};
</script>

<style lang="scss">
</style>