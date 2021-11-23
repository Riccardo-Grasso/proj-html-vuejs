<template>
  <footer>
    <!-- CONTACTS -->
    <section class="contacts pt-5 d-flex flex-column align-items-center">
      <div class="container">
        <div class="row row-cols-3">
          <div class="col col-lat pe-4">
            <img src="@/assets/footer-products.png" alt="img" class="mb-4" />
            <a class="proj-link mb-5 w-100" href="#">SHOP OUR RANGE NOW</a>
          </div>
          <div class="col central-col">
            <img src="@/assets/logo.png" alt="img" class="mb-4" />
            <div class="address text text-center mb-4">
              Avada Barbers <br />
              123 New York Street<br />
              New York City<br />
              info@yourwebsite.com<br />
              +1 (555) 555-1212
            </div>
            <div class="on-title bolder fw-bold mb-1">FOLLOW US</div>
            <div class="social-contaier">
              <a v-for="(ico, i) in socialList" :key="i" :href="ico.link">
                <i :class="ico.icon" class="p-2 fs-5 icons"></i>
              </a>
            </div>
          </div>
          <div class="col col-lat ps-4">
            <img src="@/assets/footer-image.png" alt="img" class="mb-4" />
            <a class="proj-link mb-5 w-100" href="#">BOOK YOUR APPOINTMENT</a>
          </div>
        </div>
      </div>
    </section>
    <!-- COPYRIGHT -->
    <section class="copyright">
      <div class="container py-5 text-center">
        <span class="text"
          >&copy; Copyright 2012 -2020 | Avada Theme by Themefusion | All Rights
          Reserved | Powered by WordPress</span
        >
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      socialList: [
        {
          social: "facebook",
          icon: "fa fa-facebook",
          link: "https://it-it.facebook.com/",
        },
        {
          social: "twitter",
          icon: "fa fa-twitter",
          link: "https://twitter.com/?lang=it",
        },
        {
          social: "youtube",
          icon: "fa fa-youtube-play",
          link: "https://www.youtube.com/",
        },
        {
          social: "instagram",
          icon: "fa fa-instagram",
          link: "https://www.instagram.com/",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>