<script setup>
import MainDescription from './components/MainDescription.vue';
import SecondaryDescription from './components/SecondaryDescription.vue';
import ProjectCarousel from './components/ProjectCarousel.vue';
import CustomerTestimonials from './components/CustomerTestimonials.vue';
</script>

<template>
  <main>
    <div class="wrapper">
      <MainDescription />
      <div class="aside"><ProjectCarousel /></div>
      <div class="aside hide">
        <img src="../../assets/framing.jpg" alt="" style="max-height: 750px" />
      </div>
      <SecondaryDescription />
    </div>

    <div class="featured-services">
      <CustomerTestimonials />
    </div>
    <div class="client-reviews"></div>
  </main>
</template>

<style scoped>
.aside {
  max-width: 50vw;
  position: relative;
  z-index: 1;
  overflow: hidden;
}

img {
  display: block;
}
.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-auto-rows: minmax(100px, auto);
  grid-auto-rows: 1fr;
}

@media screen and (max-width: 1250px) {
  .wrapper {
    grid-template-columns: 1fr;
    grid-auto-rows: unset;
  }
  .hide {
    display: none;
  }
  .aside {
    max-width: 100vw;
  }
}
</style>
