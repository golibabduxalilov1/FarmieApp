<template>
  <footer class="footer-section" id="footer-section">
    <div
      class="overlay d-flex flex-column justify-content-center align-items-center"
    >
      <div class="container py-5">
        <div class="row text-white">
          <!-- Company Info -->
          <div class="col-md-4">
            <img src="../assets/img/logo2.png.webp" alt="" class="mb-4" />
            <p class="footer-p mb-3 w-75">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. In act
              honcus risus atiner Pellentesque risus.
            </p>
            <p>
              <i class="bi bi-geo-alt-fill col-imp"></i> 120 Raymond Rd, New
              York
            </p>
            <p>
              <i class="bi bi-envelope-fill col-imp"></i>
              info.deercreative@gmail.com
            </p>
            <p><i class="bi bi-telephone-fill col-imp"></i> +84 223 9000</p>
          </div>

          <!-- Quick Links -->
          <div class="col-md-3">
            <h5 class="fw-bold">QUICK LINK</h5>
            <ul class="list-unstyled">
              <li><a href="#">Purchase</a></li>
              <li><a href="#">Shipping</a></li>
              <li><a href="#">Return</a></li>
              <li><a href="#">Payments</a></li>
              <li><a href="#">Guide</a></li>
              <li><a href="#">News</a></li>
            </ul>
          </div>

          <!-- Recent News -->
          <div class="col-md-3">
            <h5 class="fw-bold">RECENT NEWS</h5>
            <div class="recent-news-item d-flex align-items-center mb-4">
              <img
                src="../assets/img/4.jpg.webp"
                alt="News"
                class="news-thumbnail"
              />
              <div class="ms-3">
                <p class="m-0">
                  <a href="#">WA's largest farming business on the market</a>
                </p>
                <small>18 Aug 2018</small>
              </div>
            </div>
            <div class="recent-news-item d-flex align-items-center mb-4">
              <img
                src="../assets/img/5.jpg.webp"
                alt="News"
                class="news-thumbnail"
              />
              <div class="ms-3">
                <p class="m-0">
                  <a href="#">Beef retail prices hit a record</a>
                </p>
                <small>18 Aug 2018</small>
              </div>
            </div>
          </div>

          <!-- Social Media -->
          <div class="col-md-2">
            <h5 class="fw-bold">STAY CONNECTED</h5>
            <ul class="list-unstyled">
              <li>
                <i class="bi bi-facebook col-imp"></i> <a href="#">Facebook</a>
              </li>
              <li>
                <i class="bi bi-twitter col-imp"></i> <a href="#">Twitter</a>
              </li>
              <li>
                <i class="bi bi-pinterest col-imp"></i>
                <a href="#">Pinterest</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterSection",
};
</script>

<style scoped>
/* Footer Background */
.footer-section {
  background: url("../assets/img/footer.jpg") no-repeat center center/cover;
  color: white;
}

/* Dark Overlay */
.footer-section .overlay {
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.6);
  padding: 20px;
}

/* Footer Links */
.footer-section a {
  color: white;
  text-decoration: none;
  transition: 0.3s;
}

.footer-section a:hover {
  color: #7db122;
}

/* Quick Links */
.footer-section ul {
  padding: 0;
}

.footer-section ul li {
  margin-bottom: 10px;
}

/* Recent News */
.news-thumbnail {
  width: 50px;
  height: 50px;
  border-radius: 5px;
  object-fit: cover;
}

/* Social Media Icons */
.footer-section i {
  margin-right: 10px;
  font-size: 1.2rem;
}

.footer-p {
  font-size: 14px;
}
</style>
