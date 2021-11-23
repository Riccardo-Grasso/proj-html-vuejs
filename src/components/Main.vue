<template>
  <main>
    <!-- PRO BARBERS -->
    <SectionProBarbers></SectionProBarbers>
    <!-- SERVICES -->
    <SectionServices></SectionServices>
    <!-- AVADA GROOMING PRODUCTS -->
    <SectionProducts></SectionProducts>
    <!-- REVIEWS -->
    <SectionReviews></SectionReviews>
    <!-- BLOG POSTS -->
    <SectionBlog></SectionBlog>
  </main>
</template>

<script>
import SectionProBarbers from "@/components/SectionProBarbers.vue";
import SectionServices from "@/components/SectionServices.vue";
import SectionProducts from "@/components/SectionProducts.vue";
import SectionReviews from "@/components/SectionReviews.vue";
import SectionBlog from "@/components/SectionBlog.vue";

export default {
  name: "Main",
  components: {
    SectionProBarbers,
    SectionServices,
    SectionProducts,
    SectionReviews,
    SectionBlog,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss">
</style>
