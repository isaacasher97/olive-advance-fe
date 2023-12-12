<template>
  <!-- Get In Touch -->
  <section class="contact" id="connect">
    <div class="container">
      <div class="row align-items-center">
        <div
          id="contact-logo-img"
          class="col-12 col-md-6 wow zoomIn"
          data-wow-duration="1.5s"
        >
          <img src="/src/assets/contact-img.svg" alt="Image" />
        </div>
        <div class="col-12 col-md-6 wow fadeIn" data-wow-duration="1.5s">
          <h2>Get In Touch</h2>
          <form action="">
            <div class="row">
              <div class="col-12 col-sm-6 px-1">
                <input type="text" placeholder="First Name" required />
              </div>
              <div class="col-12 col-sm-6 px-1">
                <input type="text" placeholder="Last Name" />
              </div>
              <div class="col-12 col-sm-6 px-1">
                <input type="email" placeholder="Email Address" required />
              </div>
              <div class="col-12 col-sm-6 px-1">
                <input type="tel" placeholder="Phone No." required />
              </div>
              <div class="col-12 col-sm-6 px-1">
                <input type="text" placeholder="Company Name" />
              </div>
              <div class="col-12 col-sm-6 px-1">
                <input type="text" placeholder="Loan Amount" />
              </div>
              <div id="button-send">
                <button><span>Send</span></button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
  <!-- Get In Touch End -->
</template>

<script>
export default {
  name: "ContactForm",
};
</script>

<style scoped>
/************ Contact Form Css ************/
.contact {
  background-color: #166d3b;
  background-image: linear-gradient(147deg, #166d3b 0%, #000000 74%);
  padding: 60px 0 200px 0;
}
.contact img {
  width: 92%;
}
.contact h2 {
  font-size: 45px;
  font-weight: 700;
  margin-bottom: 30px;
  color: #f7f7f7;
  text-align: center;
}
.contact form input,
.contact form textarea {
  width: 100%;
  background: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.5);
  border-radius: 20px;
  color: #fff;
  margin: 0 0 12px 0; /* Increased margin for better spacing */
  padding: 16px 26px; /* Adjusted padding for better readability */
  font-weight: 500;
  font-size: 18px;
  letter-spacing: 0.8px;
  transition: 0.3s ease-in-out;
}
.contact form input:focus,
.contact form textarea:focus {
  background: rgba(255, 255, 255, 1);
  color: #121212;
  border: 1px solid #121212; /* Improved contrast */
}
.contact form input::placeholder,
.contact form textarea::placeholder {
  font-size: 16px;
  font-weight: 400;
  color: #fff;
}
.contact form input:focus::placeholder,
.contact form textarea:focus::placeholder {
  color: #121212;
  opacity: 0.8;
}
.contact form button {
  font-weight: 700;
  color: #fff; /* Improved contrast */
  background-color: #21d192; /* Updated button color */
  padding: 14px 48px;
  font-size: 18px;
  margin-top: 25px;
  border-radius: 20px;
  position: relative;
  transition: 0.3s ease-in-out;
  cursor: pointer; /* Added pointer cursor */
}
.contact form button span {
  z-index: 1;
  position: relative;
}
.contact form button:hover {
  background-color: #218838; /* Darker color on hover */
  color: #fff; /* White text on hover */
}
.contact form button::before {
  content: "";
  background: rgb(24, 59, 84);
  width: 0;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  font-family: Arial, Helvetica, sans-serif;
  z-index: 0;
  transition: 0.3s ease-in-out;
  border-radius: 20px;
}
.contact form button:hover::before {
  width: 100%;
}
#button-send {
  display: flex;
  justify-content: center;
}
@media (max-width: 767px) {
  .contact h2 {
    margin-bottom: 20px;
  }
  .contact form input,
  .contact form textarea {
    border-radius: 14px;
    padding: 12px 20px; /* Adjusted padding for smaller screens */
    font-size: 15px;
  }
  .contact form input::placeholder,
  .contact form textarea::placeholder {
    font-size: 14px;
  }
  .contact form button {
    padding: 12px 40px;
    font-size: 15px;
    margin-top: 16px;
  }
  .contact img {
    width: 70%;
  }
  #contact-logo-img {
    display: flex;
    justify-content: center;
  }
}
</style>
