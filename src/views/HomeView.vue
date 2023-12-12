<template>
  <div class="home">
    <Hero />
    <InfoSection />
    <GreenBar />
    <HeroTwo />
    <GreenBar />
    <h2>Services</h2>
    <CardCarousel />
    <GreenBar />
    <h2>Apply In Minutes</h2>
    <Accordion />
    <GreenBar />
    <Jumbotron />
    <GreenBar />
    <ContactForm />
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";
import InfoSection from "../components/InfoSection.vue";
import HeroTwo from "../components/HeroTwo.vue";
import CardCarousel from "../components/CardCarousel.vue";
import Accordion from "../components/Accordion.vue";
import Jumbotron from "../components/Jumbotron.vue";
import GreenBar from "../components/GreenBar.vue";
import ContactForm from "../components/ContactForm.vue";

export default {
  name: "HomeView",
  components: {
    Hero,
    InfoSection,
    HeroTwo,
    CardCarousel,
    Accordion,
    Jumbotron,
    GreenBar,
    ContactForm,
  },
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
