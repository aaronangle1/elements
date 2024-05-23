<template>
  <div class="grid">
    <img src="../assets/cabinets.jpg" alt="" />
    <img src="../assets/framing.jpg" alt="" />
    <img src="../assets/nook.jpg" alt="" />
    <img src="../assets/trusses.jpg" alt="" />
    <img src="../assets/bath.jpg" alt="" />
    <img src="../assets/workoutroom.jpg" alt="" />
  </div>
</template>

<style>
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 20px;
  align-items: center;
  justify-items: center;
  padding: 25px 10px;
}
.grid img {
  box-shadow: 2px 2px 6px 0px rgba(0, 0, 0, 0.3);
  max-width: 100%;
}

@media screen and (max-width: 800px) {
  .grid {
    grid-template-columns: 1fr 1fr;
    grid-gap: 10px;
  }
}
@media screen and (max-width: 600px) {
  .grid {
    grid-template-columns: 1fr;
  }
}
</style>
