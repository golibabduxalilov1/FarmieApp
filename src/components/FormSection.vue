<template>
  <section class="form-section container pad-100" id="form-section">
    <div class="row align-items-center">
      <!-- Left Side: Contact Form -->
      <div class="col-md-6">
        <p class="text-uppercase text-muted small">Contact Now</p>
        <h2><span class="col-imp fw-bold">Get In Touch</span> With Us</h2>
        <div class="d-flex align-items-center mb-3">
          <img src="../assets/img/decor.png.webp" alt="" />
        </div>

        <form @submit.prevent="handleSubmit" id="contact-form">
          <div class="row g-3">
            <div class="col-md-6">
              <input
                v-model="form.name"
                type="text"
                class="form-control"
                placeholder="Your Name"
                required
              />
            </div>
            <div class="col-md-6">
              <input
                v-model="form.email"
                type="email"
                class="form-control"
                placeholder="Your Email"
                required
              />
            </div>
            <div class="col-12">
              <input
                v-model="form.subject"
                type="text"
                class="form-control"
                placeholder="Your Subject"
                required
              />
            </div>
            <div class="col-12">
              <textarea
                v-model="form.message"
                class="form-control"
                rows="4"
                placeholder="Your Message"
                required
              ></textarea>
            </div>
            <div class="col-12">
              <button type="submit" class="btn but-imp w-100">
                SEND MESSAGE
              </button>
            </div>
          </div>
        </form>
      </div>

      <!-- Right Side: Google Map -->
      <div class="col-md-6 map" :style="{ height: mapHeight }">
        <iframe
          src="http://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3154.858134856195!2d-88.2621086846829!3d41.7606103792348!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x880efeb5b3575d2b%3A0x5b4dc7e5b5dc5eb!2sE%20New%20York%20St%2C%20Aurora%2C%20IL%2C%20USA!5e0!3m2!1sen!2s!4v1705648145678"
          width="100%"
          height="100%"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        >
        </iframe>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: "",
        email: "",
        subject: "",
        message: "",
      },
      mapHeight: "480px", // Responsive map height
    };
  },
  methods: {
    handleSubmit() {
      // For now, log the form data to console
      console.log(this.form);

      // Clear form after submission
      this.form.name = "";
      this.form.email = "";
      this.form.subject = "";
      this.form.message = "";
    },
  },
};
</script>

<style scoped>
/* Leaf Icon and Line */
.bi-leaf-fill {
  font-size: 24px;
}

hr {
  border: 2px solid;
  width: 50px;
  margin: 0;
}

/* Contact Form */
.form-control {
  border-radius: 5px;
  padding: 10px;
}

textarea.form-control {
  resize: none;
}

.map {
  height: 480px;
  flex: 0 0 50% 0;
}

.but-imp {
  background-color: #77b122;
  transition-duration: 500ms;
  position: relative;
  z-index: 1;
  display: inline-block;
  min-width: 160px;
  height: 50px;
  color: #ffffff;
  border-radius: 0;
  padding: 0 30px;
  font-size: 16px;
  line-height: 48px;
  font-weight: 700;
  text-transform: uppercase;
}
</style>
