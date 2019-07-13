<template>
  <footer class="footer brand-color">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column">
          <h5 class="rs-subheader">Empresa</h5>
          <p><router-link to="/about" class="rs-quote-link">Nosotros</router-link></p>
          <p><router-link to="/contact" class="rs-quote-link" target="_blank">Contactenos</router-link></p>
        </div>
        <div class="column">
          <h5 class="rs-subheader">Más Información</h5>
          <p><router-link to="/#" class="rs-quote-link">Terminos y condiciones</router-link></p>
          <p class="rs-quote">Telefono: (+51)925-811-272</p><p class="rs-quote">Email: info@rallsecurity.com</p>
        </div>
        <div class="column">
          <h5 class="rs-subheader">Buscanos en</h5>
          <p class="rs-quote">Av. Malvinas 378</p>
        </div><div class="column">
        <h5 class="rs-subheader">Síguenos en</h5>
      </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
  @import "./../../scss/variables.sass";

  .rs-quote, .rs-quote-link{
    font-family: $roboto;
    font-size: $rs-normal;
    color: $rs-black;
  }

  .rs-quote-link:hover{
    color: #fff
  }
</style>