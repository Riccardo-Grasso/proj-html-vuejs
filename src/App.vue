<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: { Header, Main, Footer },
};
</script>

<style lang="scss">
@import "styles/app";
@import "styles/header";
@import "styles/navbar";
@import "styles/main";
@import "styles/footer";
@import "styles/variables";
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:wght@800&display=swap");
</style>
