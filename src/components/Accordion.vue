<template>
  <div id="accordion-container">
    <div id="accordion" @click="highlightAccordion">
      <!-- Accordion Item 1 -->
      <div class="card">
        <div class="card-header" id="headingOne">
          <h5 class="mb-0">
            <button
              class="btn btn-link"
              data-toggle="collapse"
              data-target="#collapseOne"
              aria-expanded="true"
              aria-controls="collapseOne"
              :class="{ active: activeAccordion === 1 }"
            >
              <span class="circle-number">1</span> Simple Application
            </button>
          </h5>
        </div>

        <div
          id="collapseOne"
          class="collapse show"
          aria-labelledby="headingOne"
          data-parent="#accordion"
        >
          <div class="card-body">
            Submit your application through our online portal or contact us
            directly via phone. To initiate the process, kindly provide three
            months' worth of business bank statements, furnish your business tax
            identification number, and complete the business application form.
            Your prompt attention to these requirements will expedite the
            commencement of our collaborative endeavors.
          </div>
        </div>
      </div>

      <!-- Accordion Item 2 -->
      <div class="card">
        <div class="card-header" id="headingTwo">
          <h5 class="mb-0">
            <button
              class="btn btn-link collapsed"
              data-toggle="collapse"
              data-target="#collapseTwo"
              aria-expanded="false"
              aria-controls="collapseTwo"
              :class="{ active: activeAccordion === 2 }"
            >
              <span class="circle-number">2</span> Review
            </button>
          </h5>
        </div>
        <div
          id="collapseTwo"
          class="collapse"
          aria-labelledby="headingTwo"
          data-parent="#accordion"
        >
          <div class="card-body">
            Explore your business financing alternatives through our online
            platform or connect with one of our experienced Business Advisors
            via phone. They will assist you in selecting the most suitable
            option tailored to meet the specific needs of your business.
          </div>
        </div>
      </div>

      <!-- Accordion Item 3 -->
      <div class="card">
        <div class="card-header" id="headingThree">
          <h5 class="mb-0">
            <button
              class="btn btn-link collapsed"
              data-toggle="collapse"
              data-target="#collapseThree"
              aria-expanded="false"
              aria-controls="collapseThree"
              :class="{ active: activeAccordion === 3 }"
            >
              <span class="circle-number">3</span>Approved and Funded Quickly
            </button>
          </h5>
        </div>
        <div
          id="collapseThree"
          class="collapse"
          aria-labelledby="headingThree"
          data-parent="#accordion"
        >
          <div class="card-body">
            Upon selecting your personalized business financing solution and
            receiving approval, our team will promptly disburse the funds to the
            business bank account on record, often within a matter of hours.
          </div>
        </div>
      </div>

      <!-- Accordion Item 4 -->
      <div class="card">
        <div class="card-header" id="headingFour">
          <h5 class="mb-0">
            <button
              class="btn btn-link collapsed"
              data-toggle="collapse"
              data-target="#collapseFour"
              aria-expanded="false"
              aria-controls="collapseFour"
              :class="{ active: activeAccordion === 4 }"
            >
              <span class="circle-number">4</span> Ongoing Working Capital
            </button>
          </h5>
        </div>
        <div
          id="collapseFour"
          class="collapse"
          aria-labelledby="headingFour"
          data-parent="#accordion"
        >
          <div class="card-body">
            Feel free to reach out to us for all your future business financing
            requirements. At Olive Advance, we continually seek innovative ways
            to foster the growth of your business.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Accordion",
  data() {
    return {
      activeAccordion: 1,
    };
  },
  methods: {
    highlightAccordion(event) {
      const button = event.target.closest("button");
      if (button) {
        this.activeAccordion = parseInt(button.dataset.index);
      }
    },
  },
};
</script>

<style scoped>
.circle-number {
  display: inline-block;
  width: 30px;
  height: 30px;
  border-radius: 50%;
  background-color: #21d192; /* rgb(33, 209, 146) */
  border: 2px solid #28a745;
  color: white;
  font-size: 16px;
  text-align: center;
  line-height: 30px;
  margin-right: 10px;
  position: relative;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  top: -3px; /* Adjust this value as needed */
}

.circle-number.active {
  background-color: #28a745;
  color: white;
}

.card-header {
  background-color: transparent; /* Set background to transparent */
}

.card-header button {
  font-weight: bold;
  font-size: 18px; /* Adjust this value as needed */
  color: #333; /* Set the desired text color */
  text-decoration: none;
}

.card {
  width: 100%;
  margin: 0px auto;
}

#accordion-container {
  width: 98%;
  margin: 0 auto;
  margin-bottom: 25px;
  border-radius: 20px;
}
</style>
