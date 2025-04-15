<template>
  <!-- Farming Practices Section -->
  <section
    class="farming-practices-section container text-center pad-100"
    id="farming-practices-section"
  >
    <p class="text-uppercase text-muted small">Make the green world</p>
    <h2>
      <span class="col-imp fw-bold">Farming Practices</span> To Preserve Land &
      Water
    </h2>
    <div class="d-flex align-items-center justify-content-center mb-4">
      <img src="../assets/img/decor2.png.webp" alt="decor2" />
    </div>

    <div class="row">
      <!-- Farming Practices List -->
      <div
        v-for="(practice, index) in farmingPractices"
        :key="index"
        class="col-md-4"
      >
        <div class="practice-card">
          <figure>
            <img
              :src="practice.image"
              :alt="practice.altText"
              class="img-fluid rounded"
            />
            <figcaption>
              <div class="circle-image">
                <img :src="practice.icon" :alt="practice.iconAltText" />
              </div>
              <h6 class="text-muted title-pcard">Farming practice for</h6>
              <h4 class="fw-bold">{{ practice.title }}</h4>
              <p class="text-muted">{{ practice.description }}</p>
            </figcaption>
          </figure>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import imageRice from "@/assets/img/14.jpg.webp";
import imageSoil from "@/assets/img/13.jpg.webp";
import imageFruit from "@/assets/img/14.jpg.webp";

import iconRice from "@/assets/img/cereal.png.webp";
import iconSoil from "@/assets/img/sprout.png.webp";
import iconFruit from "@/assets/img/vegetable.png.webp";

export default {
  data() {
    return {
      farmingPractices: [
        {
          image: imageRice,
          altText: "Rice Cultivation",
          icon: iconRice,
          iconAltText: "Rice Icon",
          title: "Improved Rice Cultivation",
          description:
            "Donec nec justo eget felis facilisis fermentum. Aliquam porttitor mauris sit amet orci.",
        },
        {
          image: imageSoil,
          altText: "Soil Improvement",
          icon: iconSoil,
          iconAltText: "Soil Icon",
          title: "Soil Improvement Techniques",
          description:
            "Donec nec justo eget felis facilisis fermentum. Aliquam porttitor mauris sit amet orci.",
        },
        {
          image: imageFruit,
          altText: "Fruit Farming",
          icon: iconFruit,
          iconAltText: "Fruit Icon",
          title: "Intensive Fruit Farming",
          description:
            "Donec nec justo eget felis facilisis fermentum. Aliquam porttitor mauris sit amet orci.",
        },
      ],
    };
  },
};
</script>

<style scoped>
/* Practice Card */
.practice-card {
  position: relative;
  text-align: center;
  margin-bottom: 40px;
  padding: 15px;
  border-radius: 10px;
  background: white;
  padding-top: 50px;
}

/* Large Image */
.practice-card img {
  height: auto;
  border-radius: 10px;
}

/* Circle Image in the Middle */
.circle-image {
  width: 80px;
  height: 80px;
  background: white;
  border-radius: 50%;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

.circle-image img {
  max-width: 100%;
  height: auto;
  object-fit: cover;
}

.title-pcard {
  padding-top: 70px;
}
</style>
