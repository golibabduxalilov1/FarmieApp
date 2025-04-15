<template>
  <!-- News Section -->
  <section class="news-section container pad-100" id="news-section">
    <div class="row">
      <!-- Left Side: Featured Article -->
      <div class="col-12 col-lg-6 mb-5">
        <div class="featured-news position-relative">
          <img
            src="../assets/img/17.jpg.webp"
            alt="Vineyard"
            class="img-fluid rounded shadow"
          />
          <div class="overlay-text">
            <small class="text-light">Post on 18 Aug 2018 / Carlos Bacca</small>
            <h4 class="fw-bold text-white">
              Why innovation is key to maintaining our export market share
            </h4>
          </div>
        </div>
      </div>

      <!-- Right Side: News Articles -->
      <div class="col-12 col-lg-6 mb-100">
        <div class="news-item p-3 mb-3 bg-white rounded shadow-sm">
          <small class="text-muted">Post on 18 Aug 2018 / Peter Crough</small>
          <h5 class="fw-bold">Rising cattle supplies see beef export lifted</h5>
          <p class="text-muted">
            Maecenas facilisis quam orci, vel porttitor arcu egestas eu...
          </p>
        </div>
        <div class="news-item p-3 mb-3 bg-white rounded shadow-sm">
          <small class="text-muted">Post on 18 Aug 2018 / Peter Crough</small>
          <h5 class="fw-bold">Cattle marts: Cows take a hit at the ringside</h5>
          <p class="text-muted">
            Maecenas facilisis quam orci, vel porttitor arcu egestas eu...
          </p>
        </div>
        <div class="news-item p-3 mb-3 bg-white rounded shadow-sm">
          <small class="text-muted">Post on 18 Aug 2018 / Peter Crough</small>
          <h5 class="fw-bold">Malting barley price set to commence</h5>
          <p class="text-muted">
            Maecenas facilisis quam orci, vel porttitor arcu egestas eu...
          </p>
        </div>
        <div class="news-item p-3 mb-3 bg-white rounded shadow-sm">
          <small class="text-muted">Post on 18 Aug 2018 / Peter Crough</small>
          <h5 class="fw-bold">Cattle marts: Cows take a hit at the ringside</h5>
          <p class="text-muted">
            Maecenas facilisis quam orci, vel porttitor arcu egestas eu...
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "NewsSection",
  data() {
    return {
      newsItems: [
        {
          title: "Rising cattle supplies see beef export lifted",
          summary:
            "Maecenas facilisis quam orci, vel porttitor arcu egestas eu...",
          author: "Peter Crough",
          date: "18 Aug 2018",
        },
        {
          title: "Cattle marts: Cows take a hit at the ringside",
          summary:
            "Maecenas facilisis quam orci, vel porttitor arcu egestas eu...",
          author: "Peter Crough",
          date: "18 Aug 2018",
        },
        {
          title: "Malting barley price set to commence",
          summary:
            "Maecenas facilisis quam orci, vel porttitor arcu egestas eu...",
          author: "Peter Crough",
          date: "18 Aug 2018",
        },
        {
          title: "Cattle marts: Cows take a hit at the ringside",
          summary:
            "Maecenas facilisis quam orci, vel porttitor arcu egestas eu...",
          author: "Peter Crough",
          date: "18 Aug 2018",
        },
      ],
    };
  },
};
</script>

<style scoped>
/* Featured News Image */
.featured-news {
  position: relative;
}

.featured-news img {
  width: 100%;
  border-radius: 10px;
}

/* Overlay Text */
.overlay-text {
  position: absolute;
  bottom: 20px;
  left: 20px;
  color: white;
  padding: 15px;
  border-radius: 5px;
}

/* News Items */
.news-item {
  transition: 0.3s;
}

.news-item:hover {
  transform: translateY(-3px);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}
</style>
