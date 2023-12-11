<template>
  <Carousel :items-to-show="1" :wrap-around="true" :breakpoints="breakpoints">
    <Slide v-for="(card, index) in cardData" :key="index">
      <div class="carousel__item">
        <div class="card" @mouseover="hoverCard" @mouseleave="unhoverCard">
          <h2 class="card-heading">{{ card.heading }}</h2>
          <ul>
            <li
              v-for="(point, pointIndex) in card.bulletPoints"
              :key="pointIndex"
            >
              <img
                style="width: 20px"
                src="https://i.imgur.com/xNmMOBD.png"
                alt="Checklist Icon"
                class="checklist-icon"
              />
              {{ point }}
            </li>
          </ul>
          <a :href="card.applyNowLink" class="apply-now-link">Apply Now</a>
        </div>
      </div>
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "WrapAround",
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data: () => ({
    isHovered: false, // Added to track hover state
    cardData: [
      {
        heading: "Merchant Cash Advance",
        bulletPoints: [
          "Advance Up To $500,000",
          "Fully Funded as fast as 24 hours",
          "Swift & Quick Application Process",
          "Flexible Payments Tailored To Your Business",
        ],
        applyNowLink: "#",
      },
      {
        heading: "Bridge Loan",
        bulletPoints: [
          "Loans Starting at $3,000 up to $1.5M",
          "Terms as long as 60 months available",
          "Automatic Payments",
          "Quick and simple application process",
        ],
        applyNowLink: "#",
      },
      {
        heading: "SBA Loan",
        bulletPoints: [
          "Loans ranging from $1,000 up to $4M",
          "Terms as long as 60 months available",
          "Automatic Monthly Payments",
          "Partially Backed By the government for business purposes",
        ],
        applyNowLink: "#",
      },
      {
        heading: "Invoice Factoring",
        bulletPoints: [
          "Advances starting at $15,000 up to $8M",
          "Terms ranging up to 20 months",
          "Simple Online Application",
          "Convert pending invoices into immediate funds",
        ],
        applyNowLink: "#",
      },
      {
        heading: "Asset Based Loans",
        bulletPoints: [
          "Based On Company Assets",
          "Terms beginning at $40,000 up to $8M",
          "Terms ranging from 6 months to 36 months",
          "Fixed daily, weekly, or monthly payments",
        ],
        applyNowLink: "#",
      },
      {
        heading: "Line of Credit",
        bulletPoints: [
          "Funds starting at $3,000 up to $150,000",
          "Terms up to 20 months",
          "Access your approved amount anytime",
          "Weekly Payments",
        ],
        applyNowLink: "#",
      },
      {
        heading: "Small Business Loans",
        bulletPoints: [
          "Loans up to $1M",
          "Fully Funded as fast as 24 hours",
          "Terms ranging from 3 months to 60 months",
          "Automatic Daily or weekly payments",
        ],
        applyNowLink: "#",
      },
      // Add more card data as needed
    ],
    breakpoints: {
      // 800px to 1199px
      800: {
        itemsToShow: 2,
      },
      // 1200px and up
      1200: {
        itemsToShow: 3,
      },
    },
  }),
  methods: {
    hoverCard() {
      this.isHovered = true;
    },
    unhoverCard() {
      this.isHovered = false;
    },
  },
});
</script>

<style scoped>
.carousel {
  margin: 0 auto;
  margin-top: 25px;
  margin-bottom: 25px;

  background: #183b54;
}

.card {
  padding: 20px;
  margin: 10px;
  border: 1px solid #ddd;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  box-sizing: border-box;
  transition: background-color 0.3s, color 0.3s; /* Added transition for a smooth effect */
}

.card:hover {
  background-color: #121212;
  color: #f7f7f7;
}

.checklist-icon {
  margin-right: 5px;
}

.card-heading {
  font-weight: bold;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  margin-bottom: 10px;
  display: flex;
  align-items: center;
}

.apply-now-link {
  display: block;
  margin-top: 15px;
  text-decoration: none;
  color: #007bff;
  font-weight: bold;
}

@media (max-width: 768px) {
  .card {
    width: 90%;
    margin: 10px auto;
  }
  .carousel {
    width: 90%;
    border-radius: 10px;
  }
}
</style>
