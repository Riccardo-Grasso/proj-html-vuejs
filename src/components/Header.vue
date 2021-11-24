<template>
  <header>
    <div class="my-container">
      <!-- Navbar contiene logo e icone -->
      <Navbar></Navbar>
      <!-- SEZIONE BARBER-SHOP -->
      <section class="hero-section row row-cols-2">
        <div class="col left-text d-flex">
          <h1 class="main-title section-title mb-4">Barber Shop</h1>
          <div class="line mb-4"></div>
          <p class="text mb-4">The Pinnacle of Male Grooming</p>
          <a class="proj-link w-50" href="#">LEARN MORE</a>
        </div>
        <div class="col right-img pb-5">
          <img src="../assets/header-hero.png" alt="img" class="w-100" />
        </div>
      </section>
    </div>
    <div class="cards">
      <div class="upper-card card mb-2">
        <a href="#" class="rounded">
          <div>
            <i class="fa fa-minus-square fs-3" aria-hidden="true"></i>
          </div>
          <div class="fw-bold">Demos</div>
        </a>
      </div>
      <div class="lower-card card mb-2">
        <a href="#" class="rounded">
          <div class="price fw-bold">
            <div class="dollar">$</div>
            <div class="number">39</div>
          </div>
          <div class="fw-bold sale">On Sale</div>
        </a>
      </div>
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