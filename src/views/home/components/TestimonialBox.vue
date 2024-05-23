<script setup>
const props = defineProps(['data']);
</script>

<template>
  <div class="testimonial dark-text">
    <img src="../../../assets/quote-image.webp" alt="" class="quotes" />
    <h3>
      {{ props.data.text }}
    </h3>
    <div class="avatar-wrapper f flex-center">
      <img :src="props.data.url" alt="" class="avatar" />
      <div class="name f f-center-col">
        <h4>{{ props.data.name }}</h4>
        <p class="text-secondary">Customer</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
p {
  font-size: 16px;
  line-height: 28px;
}

h3 {
  font-size: 30px;
  font-weight: 600;
  line-height: 38px;
}
.testimonial {
  position: relative;
  max-width: 700px;
}
.quotes {
  position: absolute;
  right: 0;
  top: -110px;
  top: 0px;
  z-index: -1;
  height: 120px;
}
.avatar-wrapper {
  margin-top: 30px;
}

.name {
  align-items: flex-start;
  margin-left: 15px;
}

.name p {
  text-transform: uppercase;
}

.avatar {
  height: 90px;
  border-radius: 90px;
  object-fit: cover;
  width: 90px;
}

@media screen and (max-width: 800px) {
  h3 {
    font-size: 18px;
    font-weight: 600;
    line-height: 28px;
  }

  .quotes {
    height: 80px;
  }

  .avatar {
    height: 60px;
    width: 60px;
  }
}
</style>
