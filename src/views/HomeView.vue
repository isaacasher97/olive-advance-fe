<template>
  <div class="home">
    <Hero />
    <InfoSection />
    <!-- Section: Social media -->
    <section
      class="d-flex justify-content-between p-4 text-white"
      style="background-color: #21d192"
    >
      <!-- Left -->
      <div class="me-5"></div>
      <!-- Left -->

      <!-- Right -->
      <!-- Right -->
    </section>
    <!-- Section: Social media -->
    <HeroTwo />
    <!-- Section: Social media -->
    <section
      class="d-flex justify-content-between p-4 text-white"
      style="background-color: #21d192"
    >
      <!-- Left -->
      <div class="me-5"></div>
      <!-- Left -->

      <!-- Right -->
      <!-- Right -->
    </section>
    <!-- Section: Social media -->
    <h2>Services</h2>
    <CardCarousel />
    <!-- Section: Social media -->
    <section
      class="d-flex justify-content-between p-4 text-white"
      style="background-color: #21d192"
    >
      <!-- Left -->
      <div class="me-5"></div>
      <!-- Left -->

      <!-- Right -->
      <!-- Right -->
    </section>
    <!-- Section: Social media -->
    <h2>Apply In Minutes</h2>
    <Accordion />
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";
import InfoSection from "../components/InfoSection.vue";
import HeroTwo from "../components/HeroTwo.vue";
import CardCarousel from "../components/CardCarousel.vue";
import Accordion from "../components/Accordion.vue";

export default {
  name: "HomeView",
  components: { Hero, InfoSection, HeroTwo, CardCarousel, Accordion },
};
</script>

<style scoped>
h2 {
  text-align: center;
  margin: 15px auto;
  font-family: Arial, Helvetica, sans-serif;
  color: #121212;
  font-weight: 800;
  text-decoration: underline;
}
</style>
