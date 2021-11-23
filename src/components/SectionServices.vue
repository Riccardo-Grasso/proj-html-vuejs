<template>
  <section class="services">
    <!-- #TODO forma del div -->
    <div
      class="container padding-section d-flex flex-column align-items-center"
    >
      <div class="on-title bolder fw-bold mb-1">MENS GROOMING</div>
      <h2 class="section-title mb-4">Services</h2>
      <!-- Creo elementi con un ciclo for -->
      <!--  #TODO Creare un unico componente con la lista in props -->
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
</template>

<script>
export default {
  name: "SectionServices",
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
    };
  },
};
</script>

<style lang="scss">
</style>
