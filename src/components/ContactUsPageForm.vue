<template>
  <div id="main-header">
    <h1>Contact Us Today!</h1>
  </div>
  <div id="main-container">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 mx-auto">
          <div id="form-container" class="card mt-4 mx-auto p-4 bg-light">
            <div class="card-body bg-light">
              <div class="container">
                <form
                  action="https://formspree.io/f/mqkrzbqj"
                  method="POST"
                  id="contact-form"
                  role="form"
                >
                  <div class="controls">
                    <div class="row mb-3">
                      <div class="col-md-6">
                        <div class="form-group">
                          <label for="form_name" class="text-dark"
                            >Full Name *</label
                          >
                          <input
                            id="form_name"
                            type="text"
                            name="name"
                            class="form-control"
                            placeholder="Enter your Full Name"
                            required="required"
                            data-error="Full Name is required."
                          />
                        </div>
                      </div>
                      <div class="col-md-6">
                        <div class="form-group">
                          <label for="form_lastname" class="text-dark"
                            >Company Name *</label
                          >
                          <input
                            id="form_lastname"
                            type="text"
                            name="surname"
                            class="form-control"
                            placeholder="Enter your Company Name"
                            required="required"
                            data-error="Company Name is required."
                          />
                        </div>
                      </div>
                    </div>
                    <div class="row mb-3">
                      <div class="col-md-6">
                        <div class="form-group">
                          <label for="form_email" class="text-dark"
                            >Email *</label
                          >
                          <input
                            id="form_email"
                            type="email"
                            name="email"
                            class="form-control"
                            placeholder="Enter your email"
                            required="required"
                            data-error="Valid email is required."
                          />
                        </div>
                      </div>
                      <div class="col-md-6">
                        <div class="form-group">
                          <label for="form_need" class="text-dark"
                            >Loan Amount *</label
                          >
                          <select
                            id="form_need"
                            name="need"
                            class="form-control"
                            required="required"
                            data-error="Please specify your need."
                          >
                            <option value="" selected disabled>
                              --Select Loan Amount--
                            </option>
                            <option>$0 > $10,000</option>
                            <option>$10,000 > $50,000</option>
                            <option>$50,000 > $250,000</option>
                            <option>$250,000 +</option>
                          </select>
                        </div>
                      </div>
                    </div>
                    <div class="row mb-3">
                      <div class="col-md-12">
                        <div class="form-group">
                          <label for="form_message" class="text-dark"
                            >Message</label
                          >
                          <textarea
                            id="form_message"
                            name="message"
                            class="form-control"
                            placeholder="Write your message here."
                            rows="4"
                            data-error="Please, leave us a message."
                          ></textarea>
                        </div>
                      </div>
                    </div>
                    <div class="row">
                      <div class="col-md-12">
                        <input
                          type="submit"
                          class="btn btn-success btn-send pt-2 btn-block"
                          value="Send Message"
                        />
                      </div>
                    </div>
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactUsPageForm",
};
</script>

<style scoped>
h1 {
  background: #3498db; /* Updated background color */
  color: #fff;
  margin: 0 auto;
  padding: 15px;
  text-align: center;
}

label {
  color: #555; /* Updated label color */
}

.btn-send {
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  width: 100%; /* Updated width */
  margin-top: 10px; /* Added margin top */
}

.help-block.with-errors {
  color: #ff5050;
  margin-top: 5px;
}

.card {
  margin-left: 10px;
  margin-right: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Added box shadow for a subtle lift */
}

#form-container {
  margin-bottom: 40px;
  margin-top: 40px !important;
}

#main-container,
#main-header {
  /* background: rgb(24, 59, 84); */
  background: #f4f4f4; /* Updated background color */
}
</style>
