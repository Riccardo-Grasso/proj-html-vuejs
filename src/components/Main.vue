<template>
  <main>
    <!-- PRO BARBERS -->
    <section class="pro-barber d-flex">
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
      <div class="container padding-section">
        <div class="on-title bolder fw-bold mb-1">MENS GROOMING</div>
        <h2 class="section-title mb-4">Services</h2>
        <!-- Creo elementi con un ciclo for -->
        <div class="icon-container row">
          <div
            v-for="(service, i) in servicesList"
            :key="i"
            class="col d-flex flex-column align-items-cnter"
          >
            <img
              :src="service.icon"
              alt="icon"
              :class="service.large ? 'large' : ''"
            />
            <h3>{{ service.title }}</h3>
            <p>{{ service.text }}</p>
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
          text: "Take a seat in our fine leather chairs, lean back and let us",
          large: true,
        },
        {
          icon: require("@/assets/rasoio.png"),
          title: "Beard Tidy",
          text: "Avada Barbers are experts in the  licjety split trim and hair cut. Quick but careful and ridiculously good looking.",
          large: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>