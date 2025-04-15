<template>
  <!-- Subscribe Section -->
  <section class="subscribe-section" id="subscribe-section">
    <div
      class="overlay d-flex flex-column justify-content-center align-items-center text-center"
    >
      <p class="text-uppercase text-light small">What We Do</p>
      <h2 class="text-white fw-bold mb-3">
        Our <span class="col-imp">Produce</span> Is Mainstay For Us
      </h2>
      <div class="d-flex align-items-center justify-content-center mb-3">
        <hr class="border-success w-25 me-2" />
        <img src="../assets/img/logo.webp" alt="Logo" />
        <hr class="border-success w-25 ms-2" />
      </div>
      <p class="text-white text-center w-50 mb-5">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam at diam
        convallis ligula cursus bibendum sed at enim.
      </p>

      <!-- Subscription Form -->
      <form class="d-flex subscribe-form" @submit.prevent="handleSubscribe">
        <input
          v-model="email"
          type="email"
          class="form-control"
          placeholder="Enter your email"
          required
        />
        <button type="submit" class="btn but-imp">SUBSCRIBE</button>
      </form>

      <!-- Feedback Message -->
      <div v-if="message" class="mt-3 text-light">{{ message }}</div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      message: "",
    };
  },
  methods: {
    handleSubscribe() {
      if (!this.email) {
        this.message = "Please enter a valid email address.";
        return;
      }

      // Example logic — you could replace this with an API call
      this.message = `Thank you for subscribing, ${this.email}!`;
      this.email = "";
    },
  },
};
</script>

<style scoped>
/* Fullscreen Background Section */
.subscribe-section {
  background: url("../assets/img/form-bg.png") no-repeat center center/cover;
  width: 100%;
}

/* Dark Overlay */
.overlay {
  width: 100%;
  background: rgba(0, 0, 0, 0.5); /* Dark transparent overlay */
  padding: 100px;
}

/* Leaf Icon and Line */
.bi-leaf-fill {
  font-size: 24px;
}

hr {
  border: 2px solid;
  width: 50px;
  margin: 0;
}

/* Subscription Form */
.subscribe-form {
  width: 50%;
  max-width: 600px;
  background: white;
  border-radius: 5px;
  overflow: hidden;
  margin-bottom: 30px;
}

.subscribe-form input {
  flex-grow: 1;
  border: none;
  padding: 12px;
  outline: none;
}

.subscribe-form button {
  font-weight: bold;
  border: none;
  cursor: pointer;
}
</style>
