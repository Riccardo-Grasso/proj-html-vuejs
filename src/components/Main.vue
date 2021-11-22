<template>
  <main>
    <!-- PRO BARBERS -->
    <section class="pro-barber">
      <div
        class="container d-flex flex-column align-items-center padding-section"
      >
        <div class="on-title bolder fw-bold mb-1">AWARD WINNING</div>
        <h2 class="section-title mb-4">Pro Barbers</h2>
        <a class="proj-link mb-4" href="#">MEET YOUR NEW BARBER</a>
      </div>
    </section>
    <!-- SERVICES -->
    <section class="services">
      <div
        class="container padding-section d-flex flex-column align-items-center"
      >
        <div class="on-title bolder fw-bold mb-1">MENS GROOMING</div>
        <h2 class="section-title mb-4">Services</h2>
        <!-- Creo elementi con un ciclo for -->
        <div class="icon-container row pt-5 mb-4">
          <div
            v-for="(service, i) in servicesList"
            :key="i"
            class="col d-flex flex-column align-items-center px-5"
          >
            <img
              :src="service.icon"
              alt="icon"
              :class="service.large ? 'large' : ''"
              class="mb-4"
            />
            <h3 class="title mb-4">{{ service.title }}</h3>
            <p class="paragraph text-center">{{ service.text }}</p>
          </div>
        </div>
        <a class="proj-link" href="#">READ ABOUT OUR SERVICES</a>
      </div>
    </section>
    <!-- AVADA GROOMING PRODUCTS -->
    <section
      class="products padding-section d-flex flex-column align-items-center"
    >
      <div class="on-title bolder fw-bold mb-1">WE HAVE YOU COVERED</div>
      <h2 class="section-title mb-4">Avada Grooming Products</h2>

      <div class="products-container row pt-3 mb-4 mx-5">
        <div
          v-for="(product, i) in productsList"
          :key="i"
          class="col d-flex flex-column align-items-center px-5"
        >
          <a href="#"
            ><img :src="product.img" alt="product-image" class="mb-4"
          /></a>

          <h3 class="title mb-4">{{ product.item }}</h3>
          <p class="text-golden text-center">{{ product.price }}</p>
        </div>
      </div>
      <a class="proj-link mb-5" href="#">SHOP OUR PRODUCT RANGE</a>

      <div class="container shaving-butter mt-5">
        <div class="row row-cols-2">
          <div class="col col-left">
            <img src="@/assets/shaving_butter.png" alt="" />
          </div>
          <div class="col col-right p-5">
            <div class="on-title bolder fw-bold mb-1">
              THIS MONTHS FEATURED PRODUCT
            </div>
            <h2 class="section-title mb-4">Shaving Butter</h2>
            <p class="paragraph mb-3">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione
              et maiores fugit perspiciatis optio ad officiis quo eius! Porro,
              explicabo?
            </p>
            <a class="proj-link mb-5" href="#">BUY NOW</a>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      servicesList: [
        {
          icon: require("@/assets/trimcut.png"),
          title: "Trim & Cut",
          text: "Avada Barbers are experts in the  licjety split trim and hair cut. Quick but careful and ridiculously good looking.",
          large: false,
        },
        {
          icon: require("@/assets/washndry.png"),
          title: "Wash & Dry",
          text: "Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurious fashion.",
          large: true,
        },
        {
          icon: require("@/assets/rasoio.png"),
          title: "Beard Tidy",
          text: "Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers",
          large: false,
        },
      ],
      productsList: [
        {
          img: require("@/assets/pennello.png"),
          item: "Brush",
          price: "$15.00",
        },
        {
          img: require("@/assets/scissors.png"),
          item: "Scissors",
          price: "$85.00",
        },
        {
          img: require("@/assets/oil.png"),
          item: "Hot Oil",
          price: "$15.00",
        },
        {
          img: require("@/assets/razor.png"),
          item: "Straight Razor",
          price: "$30.00",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>