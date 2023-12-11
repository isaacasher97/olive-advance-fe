<template>
  <section>
    <div id="section-container">
      <div class="section-item">
        <div>
          <img src="https://i.imgur.com/lvueVyf.png" />
          <h3>Quickly Apply</h3>
          <p>Apply for funding in 2 Minutes</p>
        </div>
      </div>
      <div class="section-item">
        <div>
          <img src="https://i.imgur.com/dyTDOAj.png" />
          <h3>Speedy Approval</h3>
          <p>Qualify For Approval Within 2 Hours</p>
        </div>
      </div>
      <div class="section-item">
        <div>
          <img src="https://i.imgur.com/190MgUi.png" />
          <h3>Fully Funded</h3>
          <p>In As Little As 24 Hours</p>
        </div>
      </div>
      <div class="section-item">
        <div>
          <img src="https://i.imgur.com/56tKhNN.png" />
          <h3>Flexible Payment Plans</h3>
          <p>Tailored Automatic Payments For Your Business Needs</p>
        </div>
      </div>
      <div class="section-item">
        <div>
          <img src="https://i.imgur.com/86nDiNf.png" />
          <h3>Select Your Loan</h3>
          <p>Choose A Custom Amount between $2K - $2M To Receive In Funding</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "InfoSection",
};
</script>

<style scoped>
h3 {
  font-weight: 800;
}

section {
  border: 1px solid #ddd; /* Border color */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Box shadow */
  padding: 20px; /* Add padding for better spacing */
  margin: 20px; /* Add margin for better spacing */
  border-radius: 8px; /* Add border radius for rounded corners */
  box-sizing: border-box;
}

#section-container {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  align-items: center;
  box-sizing: border-box;
}

.section-item {
  flex-basis: calc(33.33% - 20px);
  box-sizing: border-box;
  align-self: center;
  text-align: center;
}

@media (max-width: 768px) {
  .section-item {
    flex-basis: 100%;
  }
}
</style>
