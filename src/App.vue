<template>
  <NavBar />
  <router-view />
  <FooterSection />
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import FooterSection from "@/components/FooterSection.vue";

export default {
  name: "App",
  components: {
    NavBar,
    FooterSection,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,200..800;1,200..800&display=swap");

body {
  font-family: "Karla", sans-serif;
  padding-top: 70px; /* Adjust based on navbar height */
}
</style>
