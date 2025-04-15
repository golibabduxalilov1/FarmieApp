<template>
  <div class="home">
    <HeroSection />
    <MainSection />
    <AboutSection />
    <ProduceSection />
    <ProductsSection />
    <SubscribeSection />
    <FarmingSection />
    <TestimonialSection />
    <FormSection />
    <NewsSection />
  </div>
</template>

<script>
import HeroSection from "@/components/HeroSection.vue";
import MainSection from "@/components/MainSection.vue";
import AboutSection from "@/components/AboutSection.vue";
import ProduceSection from "@/components/ProduceSection.vue";
import ProductsSection from "@/components/ProductsSection.vue";
import SubscribeSection from "@/components/SubscribeSection.vue";
import FarmingSection from "@/components/FarmingSection.vue";
import TestimonialSection from "@/components/TestimonialSection.vue";
import NewsSection from "@/components/NewsSection.vue";
import FormSection from "@/components/FormSection.vue";

export default {
  name: "Home",
  components: {
    HeroSection,
    MainSection,
    AboutSection,
    ProduceSection,
    ProductsSection,
    SubscribeSection,
    FarmingSection,
    TestimonialSection,
    FormSection,
    NewsSection,
  },
};
</script>

<style>
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
/* Feature Icons */
.feature-icon {
  font-size: 3rem;
  color: #77b122;
  margin-bottom: 10px;
}

.pad-100 {
  padding: 100px 0;
}

.bg-green {
  background: #77b122;
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

.main-icon {
  margin-bottom: 20px !important;
}

/* Feature Icons */
.feature-icon {
  font-size: 3rem;
  color: #77b122;
  margin-bottom: 10px;
}

.col-imp {
  color: #77b122;
}

.but-imp:hover {
  background-color: #0f1112;
  color: #ffffff;
  transition: 0.3s all;
}
</style>
