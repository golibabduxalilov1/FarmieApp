<template>
  <!-- Testimonial Section -->
  <section class="testimonial-section" id="testimonial-section">
    <div
      class="overlay d-flex flex-column justify-content-center align-items-center text-center"
    >
      <div class="container">
        <div
          id="testimonialCarousel"
          class="carousel slide"
          data-bs-ride="carousel"
        >
          <div class="carousel-inner">
            <!-- Testimonial 1 -->
            <div class="carousel-item active">
              <div
                class="testimonial-content d-flex flex-column align-items-center"
              >
                <div class="quote-icon col-imp fs-1 mb-3">
                  <img src="../assets/img/quote.png.webp" alt="Quote Icon" />
                </div>
                <h5
                  class="testimonial-text text-white text-center mb-4 ms-5 me-5"
                >
                  " you for your organic products. My children like your
                  products and they use them for breakfast. We are loving the
                  pure milk, freshly fruit and of course our staple, Brown Rice
                  Bread. Your Gluten Free breads truly make me feel lighter and
                  uplifted. It's the only bread I plan to eat for the rest of my
                  life. I will use them for many years."
                </h5>
                <div
                  class="testimonial-author d-flex align-items-center justify-content-center"
                >
                  <img
                    src="../assets/img/16.jpg.webp"
                    alt="Customer"
                    class="rounded-circle"
                  />
                  <div class="text-start ms-3">
                    <h5 class="text-white fw-bold">Mrs Lara Sullivan</h5>
                    <h6 class="col-imp m-0">Customer</h6>
                  </div>
                </div>
              </div>
            </div>

            <!-- Testimonial 2 -->
            <div class="carousel-item">
              <div
                class="testimonial-content d-flex flex-column align-items-center"
              >
                <div class="quote-icon col-imp fs-1 mb-3">
                  <img src="../assets/img/quote.png.webp" alt="Quote Icon" />
                </div>
                <h5
                  class="testimonial-text text-white text-center mb-4 ms-5 me-5"
                >
                  "Thank you for your organic products. My children like your
                  products and they use them for breakfast. We are loving the
                  pure milk, freshly fruit and of course our staple, Brown Rice
                  Bread. Your Gluten Free breads truly make me feel lighter and
                  uplifted. It's the only bread I plan to eat for the rest of my
                  life. I will use them for many years."
                </h5>
                <div
                  class="testimonial-author d-flex align-items-center justify-content-center"
                >
                  <img
                    src="../assets/img/16.jpg.webp"
                    alt="Customer"
                    class="rounded-circle"
                  />
                  <div class="text-start ms-3">
                    <h5 class="text-white fw-bold">Lara Sullivan</h5>
                    <h6 class="col-imp m-0">Customer</h6>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Carousel Controls -->
          <button
            class="carousel-control-prev"
            type="button"
            data-bs-target="#testimonialCarousel"
            data-bs-slide="prev"
          >
            <i class="bi bi-arrow-left-circle fs-3 text-white"></i>
          </button>
          <button
            class="carousel-control-next"
            type="button"
            data-bs-target="#testimonialCarousel"
            data-bs-slide="next"
          >
            <i class="bi bi-arrow-right-circle fs-3 text-white"></i>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
/* Fullscreen Background Section */
.testimonial-section {
  background: url("../assets/img/15.jpg.png") no-repeat center center/cover;
  width: 100%;
}

/* Dark Overlay */
.overlay {
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5); /* Dark transparent overlay */
  padding: 100px;
}

/* Quote Icon */
.quote-icon {
  margin-top: 10px;
  flex: 0 0 70px;
  max-width: 70px;
  width: 70px;
}

/* Testimonial Text */
.testimonial-text {
  font-size: 18px;
  color: #ffffff;
  line-height: 1.5;
  font-weight: 400;
  font-size: 1.2rem;
  max-width: 100%;
  margin: 20px 0;
}

/* Customer Info */
.testimonial-author img {
  width: 90px;
  object-fit: cover;
  width: 90px;
  border-radius: 50%;
  border: 3px solid #77b122;
}

/* Carousel Controls */
.carousel-control-prev,
.carousel-control-next {
  width: auto;
  opacity: 1;
}

.carousel-control-prev i,
.carousel-control-next i {
  transition: 0.3s;
}

.carousel-control-prev i:hover,
.carousel-control-next i:hover {
  color: #7db122;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Karla", sans-serif;
  line-height: 1.3;
  font-weight: 700;
}
</style>
