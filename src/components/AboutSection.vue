<template>
  <!-- About Us Section -->
  <section class="about-section container pad-100" id="about-section">
    <div class="row align-items-center">
      <!-- Left Side: Text Content -->
      <div class="col-md-6 about-mar">
        <p class="text-uppercase text-muted small">About Us</p>
        <h2 class="mb-3">
          <span class="col-imp fw-bold">Let Us</span> Tell You Our Story
        </h2>
        <div class="d-flex align-items-center mb-4">
          <img
            src="../assets//img/decor.png.webp"
            alt="decor"
            class="img-fluid"
          />
        </div>
        <p class="text-muted mb-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam nunc
          elit, pretium atlanta urna veloci, fermentum malesuda mina. Donec
          auctor nisl nec neque sagittis, sit amet dapibus pellentesque donal
          feugiat.
        </p>
        <a class="btn but-imp" href="/about">READ MORE</a>
      </div>

      <!-- Right Side: Circular Image with Video Play Button -->
      <div class="col-md-6 text-center">
        <div class="video-container position-relative d-inline-block">
          <img
            src="../assets/img/circle.careel.png"
            alt="Video Thumbnail"
            class="img-fluid rounded-circle"
          />
          <a
            href="#video-modal"
            class="video-play position-absolute top-50 start-50 translate-middle text-white"
          >
            <i class="bi bi-play-fill fs-1"></i>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutSection", // FIXED: component name must be a string
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

/* Video Section */
.video-container {
  position: relative;
  display: inline-block;
}

.video-container img {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 50%;
}

/* Play Button */
.video-play {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: rgba(255, 255, 255, 0.8);
  border-radius: 50%;
  padding: 15px 20px;
  font-size: 24px;
  color: black;
  text-decoration: none;
  transition: 0.3s;
}

.video-play:hover {
  background: rgba(255, 255, 255, 1);
}

.about-mar {
  margin-bottom: 100px;
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

.but-imp:hover {
  background-color: #0f1112;
  color: #ffffff;
}
</style>
