<template>
  <!-- Hero Section -->
  <section class="hero hero-section mb-lg-5" id="hero-section">
    <div
      class="hero-overlay d-flex flex-column justify-content-center align-items-center text-center"
    >
      <h1 class="hero-title display-4 fw-bold text-white">
        The Hearth Of The Farm Is The True Center Of Our Universe.
      </h1>
      <p class="hero-text text-white lead mt-3 mb-4 px-3 px-md-5">
        Mauris vestibulum dolor nec lacinia facilisis. Fusce interdum sagittis
        volutpat. Praesent eget varius ligula, malesuada eleifend purus. Aenean
        euismod est at mauris mollis ultricies.
      </p>
      <a href="#contact" class="btn but-imp hero-btn"> CONTACT US </a>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>

<style scoped>
/* Fullscreen Hero Section */
.hero {
  position: relative;
  background: url("../assets/img/sidebar.png") no-repeat center center/cover;
  width: 100%;
  height: 800px;
  z-index: 1;
}

/* Dark Overlay */
.hero-overlay {
  position: absolute;

  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.4); /* Dark transparent overlay */
  padding: 20px;
}

/* Hero Text */
.hero-title {
  font-size: 3rem;
  font-weight: bold;
  color: white;
  max-width: 700px;
  line-height: 1.3;
}

.hero-text {
  color: white;
  font-size: 1.2rem;
  max-width: 600px;
  margin-top: 15px;
}

/* Contact Button */
.hero-btn {
  margin-top: 20px;
  font-size: 1.2rem;
  font-weight: bold;
}
</style>
