<script setup>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css';
import TestimonialBox from './TestimonialBox.vue';
const testimonials = [
  {
    name: 'Bob Bobbyson',
    text: 'They do great work. Would highly recommend.',
    url: 'https://assets-global.website-files.com/5fba23eb8789c3c7fcfb5f31/622fa2005a5fabed64659616_607d8ea5221240c8618ea3d1_Kirk-Du-Plessis-Avatar%20(1).png',
  },
  {
    name: 'Aaron Angle',
    text: 'I heard the owner likes BIG dinner plate nipples. Who could blame him though. Also I remember something about him and a dead dog but my memory is a little fuzzy on that one.',
    url: 'https://media.licdn.com/dms/image/C5603AQFkiyLZ8iirxQ/profile-displayphoto-shrink_200_200/0/1570664449475?e=1721865600&v=beta&t=4xczxSDu67FZkbAq-HQG1ldMfeg20iMvf2KRBitb_18',
  },
  {
    name: 'Levi Palmer',
    text: 'Literally one of the worst places to work... HANDS DOWN!',
    url: 'https://scontent.fphx2-1.fna.fbcdn.net/v/t1.6435-9/64585297_10157459251542009_2332392753280843776_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_ohc=SvXToMW2610Q7kNvgH28FBB&_nc_ht=scontent.fphx2-1.fna&oh=00_AYASM8dN6Q1ygigDSZ5HZ39RnBOaD3crY80DEP87NpyIAA&oe=66746A8F',
  },
];
</script>

<template>
  <div class="bg-light main">
    <h4 class="dark-text-secondary small">WHAT PEOPLE SAY</h4>
    <Splide
      :options="{ rewind: true, autoplay: true, arrows: false }"
      aria-label="Vue Splide Example"
    >
      <SplideSlide v-for="t in testimonials" :key="t.name" class="f f-center">
        <TestimonialBox :data="t" />
      </SplideSlide>
    </Splide>
  </div>
</template>

<style scoped>
.main {
  padding: 5rem 10rem;
  text-align: left;
  position: relative;
  z-index: 1;
  transition: background 0.3s, border 0.3s, border-radius 0.3s, box-shadow 0.3s;
}

.small {
  font-size: 13px;
  margin-bottom: 15px;
}
@media screen and (max-width: 600px) {
  .main {
    padding: 2rem;
  }
}
</style>
