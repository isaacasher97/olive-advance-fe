<template>
  <AboutBanner />
  <GreenBar />
  <AboutUs />
  <GreenBar />
  <OurVision />
  <GreenBar />
  <WhyUs />
  <GreenBar />
  <StepByStep />
  <GreenBar />
  <ContactForm />
</template>

<script>
import AboutBanner from "../components/AboutBanner.vue";
import GreenBar from "../components/GreenBar.vue";
import AboutUs from "../components/AboutUs.vue";
import OurVision from "../components/OurVision.vue";
import StepByStep from "../components/StepByStep.vue";
import WhyUs from "../components/WhyUs.vue";
import ContactForm from "../components/ContactForm.vue";
export default {
  name: "AboutView",
  components: {
    AboutBanner,
    GreenBar,
    AboutUs,
    OurVision,
    StepByStep,
    WhyUs,
    ContactForm,
  },
};
</script>

<style></style>
