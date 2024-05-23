<template>
  <Splide
    :options="{ rewind: true, autoplay: true }"
    aria-label="Vue Splide Example"
  >
    <SplideSlide>
      <img src="../../../assets/trusses.jpg" alt="Sample 1" />
    </SplideSlide>
    <SplideSlide>
      <img src="../../../assets/cabinets.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="../../../assets/nook.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="../../../assets/bath.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="../../../assets/framing.jpg" alt="Sample 2" />
    </SplideSlide>
  </Splide>
</template>

<script setup>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css';
</script>

<style scoped>
img {
  min-width: 50vw;
  max-height: 750px;
  object-fit: cover;
}

@media screen and (max-width: 1250px) {
  img {
    min-width: 100vw;
  }
}
</style>
