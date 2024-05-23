import { RouterLink } from 'vue-router';
<template>
  <div class="spacer">
    <div class="header f f-center">
      <div class="nav-items f-center">
        <RouterLink to="/" class="icon-circle icon-circle-hover">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            class="dark-text-secondary"
          >
            <path
              d="M3 13h1v7c0 1.103.897 2 2 2h12c1.103 0 2-.897 2-2v-7h1a1 1 0 0 0 .707-1.707l-9-9a.999.999 0 0 0-1.414 0l-9 9A1 1 0 0 0 3 13zm7 7v-5h4v5h-4zm2-15.586 6 6V15l.001 5H16v-5c0-1.103-.897-2-2-2h-4c-1.103 0-2 .897-2 2v5H6v-9.586l6-6z"
            ></path>
          </svg>
        </RouterLink>
        <RouterLink to="/projects" class="nav-item">Projects</RouterLink>
        <RouterLink to="/contact" class="nav-item">Contact</RouterLink>
      </div>
      <div class="contact-items f-center">
        <div class="icon-circle hide2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
          >
            <path
              d="m20.487 17.14-4.065-3.696a1.001 1.001 0 0 0-1.391.043l-2.393 2.461c-.576-.11-1.734-.471-2.926-1.66-1.192-1.193-1.553-2.354-1.66-2.926l2.459-2.394a1 1 0 0 0 .043-1.391L6.859 3.513a1 1 0 0 0-1.391-.087l-2.17 1.861a1 1 0 0 0-.29.649c-.015.25-.301 6.172 4.291 10.766C11.305 20.707 16.323 21 17.705 21c.202 0 .326-.006.359-.008a.992.992 0 0 0 .648-.291l1.86-2.171a.997.997 0 0 0-.085-1.39z"
            ></path>
          </svg>
        </div>
        <p class="hide2">(928) 792-9117</p>
        <div class="icon-circle hide">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
          >
            <path
              d="M20 4H4c-1.103 0-2 .897-2 2v12c0 1.103.897 2 2 2h16c1.103 0 2-.897 2-2V6c0-1.103-.897-2-2-2zm0 2v.511l-8 6.223-8-6.222V6h16zM4 18V9.044l7.386 5.745a.994.994 0 0 0 1.228 0L20 9.044 20.002 18H4z"
            ></path>
          </svg>
        </div>
        <p class="hide">ElementsConstructionLLC@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.spacer {
  margin-bottom: 100px;
}
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  background-color: var(--dark);
  justify-content: space-between;
  padding: 0 30px;
  z-index: 2;
}

.nav-item {
  display: inline-block;
  text-decoration: none;
  color: var(--text);
  margin: 0 15px;
  text-transform: uppercase;
  font-weight: 500;
}

.nav-item::after {
  content: '';
  display: block;
  width: 0;
  height: 2px;
  background: var(--text);
  transition: width 0.3s;
}

.nav-item:hover::after {
  width: 100%;
}

.contact-items {
  display: flex;
  justify-content: space-evenly;
  text-transform: uppercase;
  font-size: 13px;
}

.contact-items > * {
  margin: 0 8px;
}

@media screen and (max-width: 900px) {
  .hide {
    display: none;
  }
}

@media screen and (max-width: 550px) {
  .hide2 {
    display: none;
  }
}
</style>
