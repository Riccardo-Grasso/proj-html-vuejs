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

/* ===== Scrollbar CSS ===== */
/* Firefox */
* {
  scrollbar-width: thin;
  scrollbar-color: #d0a024 #000000;
}

/* Chrome, Edge, and Safari */
*::-webkit-scrollbar {
  width: 6px;
}

*::-webkit-scrollbar-track {
  background: #000000;
}

*::-webkit-scrollbar-thumb {
  background-color: #be9359;
  border-radius: 10px;
}
</style>
