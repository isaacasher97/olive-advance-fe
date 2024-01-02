<template>
  <div class="container col-xxl-8 px-4 py-5">
    <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
      <div class="col-10 col-sm-8 col-lg-6">
        <img
          src="https://i.imgur.com/oCIsEBz.png"
          class="d-block mx-lg-auto img-fluid"
          alt="company-img"
          loading="lazy"
        />
      </div>
      <div class="col-lg-6">
        <div class="lc-block mb-3">
          <div editable="rich">
            <h2 class="fw-bold display-5">
              Your Trusted Partner in Business Growth
            </h2>
          </div>
        </div>

        <div class="lc-block mb-3">
          <div editable="rich">
            <p class="lead">
              At Olive Advance, we understand that as a business owner, you are
              the expert in your field, but navigating the world of business
              financing might be uncharted territory. That's where we come in.
              With a commitment to your success, we go beyond simply cutting a
              check. Our mission is to provide small businesses throughout the
              United States with easy access to working capital, allowing you to
              focus on what you do best, which is growing your business.
            </p>
          </div>
        </div>

        <div class="lc-block d-grid gap-2 d-md-flex justify-content-md-start">
          <a class="btn btn-primary px-4 me-md-2" href="#" role="button"
            >Apply Now</a
          >

          <a
            id="call-button"
            class="btn btn-outline-secondary px-4"
            href="tel:+17183393692"
            role="button"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-telephone-fill"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"
              /></svg
          ></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutUs",
};
</script>

<style scoped>
#call-button {
  color: #121212;
}
</style>
