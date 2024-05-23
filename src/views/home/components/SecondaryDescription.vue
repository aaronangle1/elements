<template>
  <div class="bg-dark main">
    <h4 class="dark-text-secondary small">WHO WE ARE</h4>
    <h1>
      Our mission is to build <span class="bold">above</span> the standard in
      durability, quality and efficiency.
    </h1>
    <p class="dark-text-secondary">
      Built to Last the Elements. That's our motto. We are a well-established
      company specializing in building services and home improvements. With
      extensive experience as primary building contractors, we handle a variety
      of projects, large and small, including home maintenance, improvements,
      extensions, refurbishments, and new constructions.
    </p>
  </div>
</template>

<style scoped>
.main {
  padding: 5rem 5rem;
  text-align: left;
  position: relative;
  z-index: 1;
}
h1 {
  font-size: 55px;
  line-height: 72px;
  margin-bottom: 25px;
}

.bold {
  text-decoration: underline;
}

.small {
  font-size: 13px;
  margin-bottom: 15px;
}

p {
  font-size: 16px;
  line-height: 28px;
}

@media screen and (max-width: 1250px) {
  h1 {
    font-size: 35px;
    line-height: 45px;
  }
}

@media screen and (max-width: 500px) {
  .main {
    padding: 2rem;
  }
}
</style>
