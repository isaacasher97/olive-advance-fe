<template>
  <div class="home">
    <Hero />
    <InfoSection />
    <HeroTwo />
    <h2>Services</h2>
    <CardCarousel />
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";
import InfoSection from "../components/InfoSection.vue";
import HeroTwo from "../components/HeroTwo.vue";
import CardCarousel from "../components/CardCarousel.vue";

export default {
  name: "HomeView",
  components: { Hero, InfoSection, HeroTwo, CardCarousel },
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
