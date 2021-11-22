<template>
  <nav class="d-flex align-items-center justify-content-between py-4">
    <div class="logo-container">
      <img src="@/assets/logo.png" alt="logo" />
    </div>
    <div class="icon-container d-flex">
      <a v-for="(icon, i) in iconList" :key="i" :href="icon.link">
        <i :class="icon.ico" class="p-2 fs-4 icons"></i>
      </a>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      iconList: [
        { ico: "fa fa-shopping-cart", link: "#" },
        { ico: "fa fa-bars", link: "#" },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>