<template>
  <!-- Main Section -->
  <section
    class="main-section container text-center mt-3 pad-100"
    id="main-section"
  >
    <!-- Large Farm Image -->
    <div class="row justify-content-center mb-5">
      <div class="col-md-10">
        <img
          src="../assets/img/2.jpg.webp"
          alt="Scenic view of a farm"
          class="img-fluid rounded shadow"
        />
      </div>
    </div>

    <!-- Feature Icons Section -->
    <div class="row text-center">
      <div
        v-for="(feature, index) in features"
        :key="index"
        class="col-md-2"
        :class="{ 'offset-md-1': index === 0 }"
      >
        <img :src="feature.img" :alt="feature.alt" class="main-icon mb-2" />
        <h5>{{ feature.label }}</h5>
      </div>
    </div>
  </section>
</template>

<script>
import imgDigger from "@/assets/img/digger.png.webp";
import imgWindmill from "@/assets/img/windmill.png.webp";
import imgCereals from "@/assets/img/cereals.png.webp";
import imgTractor from "@/assets/img/tractor.png.webp";
import imgSunrise from "@/assets/img/sunrise.png.webp";

export default {
  name: "MainSection",
  data() {
    return {
      features: [
        {
          img: imgDigger,
          alt: "Digger icon",
          label: "Best Services",
        },
        {
          img: imgWindmill,
          alt: "Windmill icon",
          label: "Farm Experiences",
        },
        {
          img: imgCereals,
          alt: "Cereals icon",
          label: "100% Natural",
        },
        {
          img: imgTractor,
          alt: "Tractor icon",
          label: "Farm Equipment",
        },
        {
          img: imgSunrise,
          alt: "Sunrise icon",
          label: "Organic Food",
        },
      ],
    };
  },
};
</script>

<style scoped>
.main-icon {
  margin-bottom: 20px !important;
}

.feature-icon {
  font-size: 3rem;
  color: #77b122;
  margin-bottom: 10px;
}
</style>
