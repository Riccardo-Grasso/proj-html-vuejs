<template>
  <header>
    <div class="container">
      <Navbar></Navbar>
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