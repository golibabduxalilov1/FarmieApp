<template>
  <!-- Our Produce Section -->
  <section class="produce-section container pad-100" id="produce-section">
    <div class="row align-items-center">
      <!-- Left Side: Image -->
      <div class="col-md-6 mb-4 mb-md-0">
        <img
          src="../assets/img/product.png"
          alt="Fresh produce on display"
          class="img-fluid rounded shadow"
        />
      </div>

      <!-- Right Side: Text & Features -->
      <div class="col-md-6 ps-md-5">
        <p class="text-uppercase text-muted small">What We Do</p>
        <h1 class="fw-bold mb-3">
          <span class="col-imp">Our Produce</span> Is Mainstay For Us
        </h1>

        <div class="d-flex align-items-center mb-3">
          <img src="../assets/img/decor.png.webp" alt="Brand logo" />
        </div>

        <p class="text-muted mb-4">
          Mauris fermentum nunc quis massa lacinia consequat. Suspendisse orci
          magna, pharetra sedonia risus ut, elementum mollis nisi. Nunc in
          sapien turpis. Donec egeto david orci pulvinar ultrices.
        </p>

        <!-- Feature Items -->
        <div class="row">
          <div
            class="col-6 mb-4"
            v-for="feature in features"
            :key="feature.title"
          >
            <i :class="feature.icon + ' col-imp feature-icon mb-2 d-block'"></i>
            <h5>{{ feature.title }}</h5>
            <p class="text-muted small">{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      features: [
        {
          icon: "bi bi-flower1",
          title: "Fruit & Vegetable",
          description: "Intiam eu sagittis est, aster cosmo lacini libero.",
        },
        {
          icon: "bi bi-egg-fried",
          title: "Meat & Eggs",
          description: "Intiam eu sagittis est, aster cosmo lacini libero.",
        },
        {
          icon: "bi bi-basket3",
          title: "Milk & Cheese",
          description: "Intiam eu sagittis est, aster cosmo lacini libero.",
        },
        {
          icon: "bi bi-flower2",
          title: "Rice & Corn",
          description: "Intiam eu sagittis est, aster cosmo lacini libero.",
        },
      ],
    };
  },
};
</script>

<style scoped>
.feature-icon {
  font-size: 2rem;
}
.pad-100 {
  padding: 100px 0;
}
</style>
