<template>
  <section
    class="products padding-section d-flex flex-column align-items-center"
  >
    <div class="on-title bolder fw-bold mb-1">WE HAVE YOU COVERED</div>
    <h2 class="section-title mb-4">Avada Grooming Products</h2>

    <div class="products-container row pt-3 mb-5 mx-5">
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
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione et
            maiores fugit perspiciatis optio ad officiis quo eius! Porro,
            explicabo?
          </p>
          <a class="proj-link w-50 mb-5" href="#">BUY NOW</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionProducts",
  data() {
    return {
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