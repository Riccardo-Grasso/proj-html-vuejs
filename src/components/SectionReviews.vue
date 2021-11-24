<template>
  <section class="reviews">
    <div
      class="my-container padding-section d-flex flex-column align-items-center"
    >
      <div class="on-title bolder fw-bold mb-1">WHAT PEOPLE SAY</div>
      <h2 class="section-title mb-4">Reviews</h2>

      <div class="icon-container row pt-5 mb-4">
        <div
          v-for="(review, i) in reviewsList"
          :key="i"
          class="col d-flex flex-column align-items-center px-5"
        >
          <p class="paragraph text-center">{{ review.text }}</p>
          <img
            :src="review.photo"
            alt="photo"
            class="mb-4 w-50 rounded-circle"
          />
          <h6 class="text-golden mb-4 fst-italic">{{ review.name }}</h6>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionReviews",
  data() {
    return {
      reviewsList: [
        {
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos enim quia quasi? Suscipit quam quaerat nihil quo aspernatur consectetur, numquam ipsam, facere asperiores praesentium.",
          photo: require("@/assets/client-1.jpg"),
          name: "John Doe",
        },
        {
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos enim quia quasi? Suscipit quam quaerat nihil quo aspernatur consectetur, numquam ipsam, facere asperiores praesentium.",
          photo: require("@/assets/client-2.jpg"),
          name: "Pete Jones",
        },
        {
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos enim quia quasi? Suscipit quam quaerat nihil quo aspernatur consectetur, numquam ipsam, facere asperiores praesentium.",
          photo: require("@/assets/client-3.jpg"),
          name: "Mark Wilson",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>
