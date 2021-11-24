<template>
  <section class="blog">
    <img class="triangolo" src="@/assets/triangle-white.svg" alt="triangolo" />
    <div
      class="my-container padding-section d-flex flex-column align-items-center"
    >
      <div class="on-title bolder fw-bold mb-1">TALES FROM THE BARBER SHOP</div>
      <h2 class="section-title mb-4">Recent Blog Posts</h2>
      <div class="blog-container row row-cols-3 pt-5 mb-4">
        <div
          v-for="(post, i) in postsList"
          :key="i"
          class="col d-flex flex-column align-items-center p-3"
        >
          <img :src="post.img" alt="post-img" class="mb-4 w-100" />
          <h3 class="title mb-4 text-center">{{ post.title }}</h3>
          <p class="paragraph text-center">{{ post.text }}</p>
        </div>
      </div>
      <a class="proj-link" href="#">READ MORE FROM OUR BLOG</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionBlog",
  data() {
    return {
      postsList: [
        {
          img: require("@/assets/blog1.jpg"),
          title: "Avada Barbers Now Open",
          text: "Avada Barbers are experts in the  licjety split trim and hair cut. Quick but careful and ridiculously good looking.",
        },
        {
          img: require("@/assets/blog2.jpg"),
          title: "Choosing The Right Barber",
          text: "Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurious fashion.",
        },
        {
          img: require("@/assets/blog3.jpg"),
          title: "Quick Service Guide",
          text: "Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers",
        },
      ],
    };
  },
};
</script>


<style lang="scss">
</style>
