<template>
  <div class="main f-center">
    <div class="box dark-text">
      <h1>Looking for a quote for your next construction project?</h1>
      <p>Contact us and we'll get in touch with you as soon as possible.</p>
      <div class="line"></div>
      <div class="f-center start">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="48"
          height="48"
          viewBox="0 0 24 24"
          class=""
        >
          <path
            d="m20.487 17.14-4.065-3.696a1.001 1.001 0 0 0-1.391.043l-2.393 2.461c-.576-.11-1.734-.471-2.926-1.66-1.192-1.193-1.553-2.354-1.66-2.926l2.459-2.394a1 1 0 0 0 .043-1.391L6.859 3.513a1 1 0 0 0-1.391-.087l-2.17 1.861a1 1 0 0 0-.29.649c-.015.25-.301 6.172 4.291 10.766C11.305 20.707 16.323 21 17.705 21c.202 0 .326-.006.359-.008a.992.992 0 0 0 .648-.291l1.86-2.171a.997.997 0 0 0-.085-1.39z"
          ></path>
        </svg>
        <p class="contact">(928) 792-9117</p>
      </div>

      <div class="f-center start mt">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="48"
          height="48"
          viewBox="0 0 24 24"
          class="mr"
        >
          <path
            d="M20 4H4c-1.103 0-2 .897-2 2v12c0 1.103.897 2 2 2h16c1.103 0 2-.897 2-2V6c0-1.103-.897-2-2-2zm0 2v.511l-8 6.223-8-6.222V6h16zM4 18V9.044l7.386 5.745a.994.994 0 0 0 1.228 0L20 9.044 20.002 18H4z"
          ></path>
        </svg>
        <p class="upper contact">ElementsConstructionLLC@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<style>
.main {
  padding: 90px 0;
  min-height: 60vh;
}

.box {
  background-color: var(--white);
  position: relative;
  padding: 35px;
  border-radius: 15px;
  align-items: flex-start;
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
  margin: 0 5px;
}
.line {
  background-color: var(--text-secondary);
  width: 100%;
  height: 2px;
  margin: 20px 0;
}
.start {
  justify-content: flex-start;
}

.contact {
  font-size: 20px;
  margin-left: 15px;
}

.upper {
  text-transform: uppercase;
}

.mt {
  margin-top: 30px;
}

@media screen and (max-width: 550px) {
  .contact {
    font-size: 14px;
    margin-top: 5px;
  }
  .start {
    flex-direction: column;
  }
  .box {
    padding: 20px;
  }
}
</style>
