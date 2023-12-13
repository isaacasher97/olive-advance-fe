<template>
  <h2 id="why-us-header">Why Us?</h2>
  <div class="container py-5 timeline position-relative">
    <div class="timeline-item w-100 mb-4 py-4 text-dark lc-block">
      <div class="timeline-img bg-primary"></div>
      <div class="timeline-content">
        <img style="width: 70px" src="../assets/title-logo.png" />
        <h2 editable="inline" class="fw-bold rfs-12">Expert Guidance</h2>
        <div editable="rich">
          <p>
            Unlike some capital funding organizations, our financial experts are
            well-versed in business financing. We help you navigate through the
            maze of financing options, making sense of the technical jargon that
            can often be overwhelming.
          </p>
        </div>
      </div>
    </div>
    <div class="timeline-item w-100 mb-4 py-4 text-dark lc-block">
      <div class="timeline-img bg-success"></div>
      <div class="timeline-content">
        <img style="width: 70px" src="../assets/title-logo.png" />
        <h2 editable="inline" class="fw-bold rfs-12">Proven Track Record</h2>
        <div editable="rich">
          <p>
            Don't just take our word for it – our track record speaks for
            itself. With over 4.6 stars on Trustpilot and glowing testimonials,
            our commitment to quick, painless business loans, experienced
            professionals, and stellar customer service is evident.
          </p>
        </div>
      </div>
    </div>
    <div class="timeline-item w-100 mb-4 py-4 text-dark lc-block">
      <div class="timeline-img bg-warning"></div>
      <div class="timeline-content">
        <img style="width: 70px" src="../assets/title-logo.png" />
        <h2 editable="inline" class="fw-bold rfs-12">
          Client-Centric Approach
        </h2>
        <div editable="rich">
          <p>
            We take the time to understand your specific funding needs. Our
            streamlined application process ensures that you receive an offer
            within hours of submission, and upon approval, funds can be in your
            account within 24 hours.
          </p>
        </div>
      </div>
    </div>
    <div class="timeline-item w-100 mb-4 py-4 text-dark lc-block">
      <div class="timeline-img bg-info"></div>
      <div class="timeline-content">
        <img style="width: 70px" src="../assets/title-logo.png" />
        <h2 editable="inline" class="fw-bold rfs-12">Tailored Solutions</h2>
        <div editable="rich">
          <p>
            At Olive Advance, we understand that every business is unique.
            That's why we provide tailored financing solutions designed to meet
            the specific needs of your business. Our goal is not just to provide
            funding but to support your growth with solutions that align with
            your business objectives.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WhyUs",
};
</script>

<style scoped>
#why-us-header {
  text-align: center;
  padding: 10px;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 600;
  text-decoration: underline;
}

.timeline:before {
  content: "";
  background: var(--bs-secondary);
  width: 5px;
  height: 95%;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}
.timeline-item:nth-child(even) .timeline-content {
  float: right;
  padding: 40px 30px 10px 30px;
}
.timeline-item:nth-child(even) .timeline-content .date {
  right: auto;
  left: 0;
}
.timeline-item:nth-child(even) .timeline-content::after {
  content: "";
  position: absolute;
  border-style: solid;
  width: 0;
  height: 0;
  top: 30px;
  left: -15px;
  border-width: 10px 15px 10px 0;
  border-color: transparent var(--bs-light) transparent transparent;
}
.timeline-item::after {
  content: "";
  display: block;
  clear: both;
}
.timeline-content {
  position: relative;
  width: 45%;
  padding: 10px 30px;
  border-radius: 4px;
  background: rgb(24, 59, 84);
  color: #f7f7f7;
  transition: background-color 0.3s;
}
.timeline-content:hover {
  background-color: #f0f0f0;
  color: #121212;
}
.timeline-content::after {
  content: "";
  position: absolute;
  border-style: solid;
  width: 0;
  height: 0;
  top: 30px;
  right: -15px;
  border-width: 10px 0 10px 15px;
  border-color: transparent transparent transparent var(--bs-light);
}
.timeline-img {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  position: absolute;
  left: 50%;
  margin-top: 25px;
  margin-left: -15px;
  transition: background-color 0.3s;
}
.timeline-img:hover {
  background-color: #dcdcdc;
}
@media screen and (max-width: 768px) {
  .timeline::before {
    left: 50px;
  }
  .timeline .timeline-img {
    left: 50px;
  }
  .timeline .timeline-content {
    max-width: 100%;
    width: auto;
    margin-left: 70px;
  }
  .timeline .timeline-item:nth-child(even) .timeline-content {
    float: none;
  }
  .timeline .timeline-item:nth-child(odd) .timeline-content::after {
    content: "";
    position: absolute;
    border-style: solid;
    width: 0;
    height: 0;
    top: 30px;
    left: -15px;
    border-width: 10px 15px 10px 0;
    border-color: transparent #f5f5f5 transparent transparent;
  }
}
</style>
