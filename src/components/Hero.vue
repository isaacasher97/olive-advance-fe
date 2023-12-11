<template>
  <div id="hero">
    <div
      lc-helper="background"
      class="container-fluid py-5 mb-4 d-flex justify-content-center"
      style="
        background-image: url('https://images.unsplash.com/photo-1600880292203-757bb62b4baf?q=80&w=2340&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
      "
    >
      <div
        class="p-5 mb-4 lc-block col-xxl-7 col-lg-8 col-12"
        style="
          backdrop-filter: blur(2px) saturate(102%);
          -webkit-backdrop-filter: blur(6px) saturate(102%);
          background-color: rgba(0, 0, 0, 0.45);
          border-radius: 12px;
          border: 1px solid rgba(209, 213, 219, 0.3);
        "
      >
        <div class="lc-block">
          <div editable="rich">
            <h2 class="fw-bolder display-4">
              An alternative approach to business financing
            </h2>
          </div>
        </div>
        <div class="lc-block col-md-8">
          <div editable="rich">
            <p class="lead">
              Explore rapid and straightforward business funding solutions with
              Olive Advance. Our dedication is to simplify the process, making
              business funding an easy, seamless experience. Receive a
              personalized quote within minutes.
            </p>
          </div>
        </div>
        <div id="apply-button" class="lc-block">
          <button class="bn47">
            <a href="#" role="button">Apply Now</a>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style scoped>
@media (min-width: 768px) {
  .col-md-8 {
    width: 100%;
  }
}

h2,
p {
  color: #f7f7f7;
  font-family: Arial, Helvetica, sans-serif;
}

h2,
a {
  text-align: center;
}

button {
  background-color: #183b54;
}

/* .btn {
  display: flex;
  justify-content: center;
  width: 50%;
  margin: 0 auto;
} */

#apply-button {
  display: flex;
  justify-content: center;
  width: 100%;
  margin: 0 auto;
}

/* button styling  */
.bn47 {
  position: relative;
  padding: 1rem 2rem 0.5rem 2.5rem;
  color: #000000;
  border: 1px dashed #f7f7f7;
  -webkit-transition: padding 0.3s ease-in-out;
  transition: padding 0.3s ease-in-out;
}

.bn47:before {
  content: "";
  position: absolute;
  top: 0.5rem;
  left: 0.5rem;
  z-index: -1;
  height: 100%;
  width: 100%;
  background-color: #183b54;
  border-right: 3px solid #183b54;
  border-bottom: 3px solid #183b54;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

.bn47:hover {
  padding: 0.75rem 2.25rem;
}

.bn47:hover:before {
  top: 0;
  left: 0;
}

a {
  text-decoration: #183b54;
  color: #f7f7f7;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 800;
}
/* button styling end  */

.mb-4 {
  margin-bottom: 0 !important;
}
</style>
