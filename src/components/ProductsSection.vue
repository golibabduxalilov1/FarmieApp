<template>
  <!-- Featured Products Section -->
  <section
    class="featured-products-section container text-center pad-100"
    id="featured-products-section"
  >
    <p class="text-uppercase text-muted small">Featured Products</p>
    <h2>
      <span class="col-imp fw-bold">Our Product</span> Are Highest Quality
    </h2>
    <div class="d-flex align-items-center justify-content-center mb-4">
      <img src="../assets/img/decor2.png.webp" alt="decor2" />
    </div>

    <!-- Product Grid -->
    <div class="row">
      <!-- Product 1 -->
      <div class="col-md-3" v-for="(product, index) in products" :key="index">
        <div class="product-card">
          <span v-if="product.badge" :class="'badge ' + product.badgeClass">{{
            product.badge
          }}</span>
          <img :src="product.img" :alt="product.name" />
          <h5>{{ product.name }}</h5>
          <p class="price" v-if="!product.oldPrice">${{ product.price }}</p>
          <p class="price" v-else>
            <s class="text-muted">${{ product.oldPrice }}</s>
            <strong>${{ product.price }}</strong>
          </p>
          <div class="product-actions">
            <button class="btn btn-light"><i class="bi bi-heart"></i></button>
            <button class="btn btn-light"><i class="bi bi-cart"></i></button>
            <button class="btn btn-light">
              <i class="bi bi-arrow-left-right"></i>
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Store Button -->
    <div class="mt-4">
      <a href="#" class="btn but-imp">GO TO STORE</a>
    </div>
  </section>
</template>

<script>
import strawberryImg from "@/assets/img/p1.jpg.webp";
import bakedBreadsImg from "@/assets/img/p2.jpg.webp";
import primeBeefImg from "@/assets/img/p3.jpg.webp";
import pureHoneyImg from "@/assets/img/p4.jpg.webp";

export default {
  data() {
    return {
      products: [
        {
          name: "Strawberry",
          price: 17.99,
          img: strawberryImg,
          badge: "HOT",
          badgeClass: "bg-success",
        },
        {
          name: "Baked Breads",
          price: 9.99,
          img: bakedBreadsImg,
        },
        {
          name: "Prime Beef",
          price: 59.99,
          img: primeBeefImg,
        },
        {
          name: "Pure Honey",
          price: 19.99,
          oldPrice: 29.99,
          img: pureHoneyImg,
          badge: "SALE",
          badgeClass: "bg-danger",
        },
      ],
    };
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
  width: 25%;
  margin: 0;
}

/* Product Cards */
.product-card {
  position: relative;
  background: #f8f8f8;
  padding: 20px;
  border-radius: 8px;
  text-align: center;
  transition: 0.3s;
}

.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

/* Product Images */
.product-card img {
  width: 100%;
  height: auto;
  margin-bottom: 10px;
}

/* Product Price */
.price {
  font-size: 18px;
  font-weight: bold;
  margin-top: 5px;
}

/* Product Labels */
.badge {
  position: absolute;
  top: 10px;
  left: 10px;
}

/* Product Actions */
.product-actions {
  margin-top: 10px;
}

.product-actions .btn {
  margin: 5px;
}
</style>
