<template>
  <nav
    class="navbar navbar-expand-lg navbar-light bg-white shadow-sm fixed-top"
  >
    <div class="container">
      <!-- Logo -->
      <router-link class="navbar-brand fw-bold text-success" to="/">
        <img src="../assets/img/logo.png.webp" alt="logo" />
      </router-link>

      <!-- Toggle Button for Mobile -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Navigation Links -->
      <div class="collapse navbar-collapse fade-in" id="navbarNav">
        <ul class="navbar-nav mx-auto">
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#hero-section') }"
              to="/#hero-section"
            >
              HOME
            </router-link>
          </li>
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#about-section') }"
              to="/#about-section"
            >
              ABOUT
            </router-link>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="pagesDropdown"
              role="button"
              data-bs-toggle="dropdown"
            >
              PAGES
            </a>
            <ul class="dropdown-menu animate-dropdown">
              <li>
                <router-link class="dropdown-item" to="/">Page 1</router-link>
              </li>
              <li>
                <router-link class="dropdown-item" to="/">Page 2</router-link>
              </li>
              <li>
                <router-link class="dropdown-item" to="/">Page 3</router-link>
              </li>
            </ul>
          </li>
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#featured-products-section') }"
              to="/#featured-products-section"
            >
              OUR PRODUCT
            </router-link>
          </li>
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#farming-practices-section') }"
              to="/#farming-practices-section"
            >
              FARMING PRACTICE
            </router-link>
          </li>
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#news-section') }"
              to="/#news-section"
            >
              NEWS
            </router-link>
          </li>
          <li class="nav-item">
            <router-link
              class="nav-link"
              :class="{ 'col-imp': isActive('#footer-section') }"
              to="/#footer-section"
            >
              CONTACT
            </router-link>
          </li>
        </ul>

        <!-- Search and Cart Icons -->
        <div class="d-flex align-items-center">
          <a href="#" class="me-3 text-dark"><i class="bi bi-search"></i></a>
          <a
            href="#"
            class="position-relative text-dark"
            @click="incrementCart"
          >
            <i class="bi bi-cart"></i>
            <span
              class="cart-badge position-absolute top-0 start-100 translate-middle badge rounded-pill bg-green"
            >
              {{ cartCount }}
            </span>
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      cartCount: 2,
    };
  },
  methods: {
    isActive(section) {
      return window.location.hash === section;
    },
    incrementCart() {
      this.cartCount++;
    },
  },
};
</script>
<style>
/* General Navbar Styling */
.navbar {
  padding: 15px 0;
}

/* Ensure the navbar remains fixed at the top */
.fixed-top {
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1030; /* Ensures it stays above other elements */
}

/* Add some padding to the body to prevent content from hiding under the navbar */

/* Navbar Hover Effect */
.navbar-nav .nav-link {
  transition: color 0.3s ease-in;
}

.navbar-nav .nav-link:hover {
  color: #77b122;
}

/* Shopping Cart Badge */
.cart-badge {
  font-size: 12px;
  padding: 3px 6px;
}

.col-imp {
  color: #77b122 !important;
}
</style>
