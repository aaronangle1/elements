<template>
  <div class="dark-text main f-center-col">
    <img src="../../../assets/tinyhouseplan.png" alt="" />
    <div class="box f-center-col">
      <h1>Elements Construction</h1>
      <p class="text-secondary">
        The Gila Valley's Premier Construction Company
      </p>
      <RouterLink to="/contact" class="button">
        Contact
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="20"
          height="20"
          viewBox="0 0 24 24"
          class="arrow"
        >
          <path
            d="M21 11H6.414l5.293-5.293-1.414-1.414L2.586 12l7.707 7.707 1.414-1.414L6.414 13H21z"
          ></path>
        </svg>
      </RouterLink>
    </div>
  </div>
</template>

<style scoped>
.main {
  min-height: 600px;
}
img {
  height: 800px;
  transform: rotate(-25deg);
  position: fixed;
  top: 0px;
  left: -80px;
  z-index: 0;
  opacity: 0.4;
}
.box {
  background-color: var(--white);
  position: relative;
  padding: 35px;
  border-radius: 15px;
  align-items: flex-start;
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
}

.box h1 {
  font-size: 52px;
}
.button {
  background-color: transparent;
  text-decoration: none;
  border: solid 3px var(--border);
  padding: 10px 15px;
  border-radius: 50px;
  transition: 0.3s;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 13px;
  margin-top: 35px;
}

.arrow {
  fill: var(--dark);
  transform: rotate(135deg);
  position: relative;
  top: 5px;
}

.button:hover {
  background-color: var(--dark);
  border-color: var(--dark);
  color: var(--light);
}

.button:hover .arrow {
  fill: var(--light) !important;
}

@media screen and (max-width: 700px) {
  .box h1 {
    font-size: 40px;
  }
}

@media screen and (max-width: 500px) {
  .box h1 {
    font-size: 30px;
  }
}
</style>
