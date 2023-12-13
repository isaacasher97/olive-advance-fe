<template>
  <ContactBanner />
  <GreenBar />
  <ContactUsPageForm />
  <ContactCard />
</template>

<script>
import ContactBanner from "../components/ContactBanner.vue";
import GreenBar from "../components/GreenBar.vue";
import ContactUsPageForm from "../components/ContactUsPageForm.vue";
import ContactCard from "../components/ContactCard.vue";
export default {
  name: "ContactView",
  components: { ContactBanner, GreenBar, ContactUsPageForm, ContactCard },
};
</script>

<style></style>
