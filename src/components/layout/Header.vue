<template>
  <section>
    <nav role="navigation" aria-label="main navigation" class="navbar">
      <div class="navbar-brand">
        <router-link to="/" class="navbar-item brand-title router-link-exact-active router-link-active">
          Rall Security
        </router-link>
        <a role="button" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample" class="navbar-burger burger">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>
      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start"><div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link">
            Catalogo
          </a>
          <div class="navbar-dropdown">
            <div class="nested navbar-item dropdown">
              <div class="dropdown-trigger">
                <button aria-haspopup="true" aria-controls="dropdown-menu" class="button">
                  <span>Contrucción</span>
                  <span class="icon is-small"><i aria-hidden="true" class="fas fa-angle-down"></i>
                  </span></button>
              </div>

              <div id="dropdown-menu" role="menu" class="dropdown-menu">
                <div class="dropdown-content">
                  <div class="nested navbar-item dropdown">
                    <div class="dropdown-trigger">
                      <button aria-haspopup="true" aria-controls="dropdown-menu" class="button">
                        <span>Protectores</span>
                        <span class="icon is-small"><i aria-hidden="true" class="fas fa-angle-down"></i>
                        </span></button>
                    </div>
                    <div id="dropdown-menu" role="menu" class="dropdown-menu">
                      <div class="dropdown-content">
                        <router-link to="/catalog" class="dropdown-item">Cabeza</router-link>
                        <router-link to="/catalog" class="dropdown-item">Visual</router-link>
                        <router-link to="/catalog" class="dropdown-item">Oidos</router-link>
                        <router-link to="/catalog" class="dropdown-item">Nasal</router-link>
                        <router-link to="/catalog" class="dropdown-item">Indumentaria</router-link>
                        <router-link to="/catalog" class="dropdown-item">Anticaídas</router-link>
                        <router-link to="/catalog" class="dropdown-item">Manos</router-link>
                        <router-link to="/catalog" class="dropdown-item">Calzado</router-link>
                      </div>
                    </div>
                  </div>
                  <router-link to="/catalog" class="dropdown-item">Señalizaciones</router-link>
                </div>
              </div>
            </div>

            <div class="nested navbar-item dropdown">
              <div class="dropdown-trigger">
                <button aria-haspopup="true" aria-controls="dropdown-menu" class="button">
                  <span>Privado</span>
                  <span class="icon is-small"><i aria-hidden="true" class="fas fa-angle-down"></i></span>
                </button>
              </div>
              <div id="dropdown-menu" role="menu" class="dropdown-menu">
                <div class="dropdown-content">
                  <router-link to="/catalog" class="dropdown-item">Vigilancia</router-link>
                  <router-link to="/catalog" class="dropdown-item">Limpieza</router-link>
                  <router-link to="/catalog" class="dropdown-item">Accesorios</router-link>
                </div>
              </div>
            </div>
          </div>
        </div>
        </div>

        <div class="navbar-end">
          <router-link to="/" class="navbar-item router-link-exact-active router-link-active">Inicio</router-link>
          <router-link to="/about" class="navbar-item">Nosotros</router-link>
          <router-link to="/contact" class="navbar-item" target="_blank">Contacto</router-link>
        </div>
      </div>
    </nav>
  </section>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>

</style>