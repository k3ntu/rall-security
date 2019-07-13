<template>
  <div class="rs-body-white pb-section">
    <main class="main-background is-vertical-center">
      <div class="container is-fluid">
        <div class="columns is-vcentered">
          <div class="column is-4 is-offset-1">
            <h1 class="main-title">Confortable y seguro. Protege tu futuro y el de tu familia.</h1>
            <p class="main-subtitle">Descubre la calidad de nuestros productos</p>
            <a href="/catalog" class="button is-fullwidth is-warning is-inverted is-outlined rs-montserrat rs-semibold">
              VER AHORA
            </a>
          </div>
          <div class="column is-4 is-offset-1">
            <figure class="image">
              <img src="/img/main-photo.jpg" alt="Foto principal">
            </figure>
          </div>
        </div>
      </div>
    </main>

    <div class="container mb-section">
      <h2 class="main-title">Catalogo</h2>
      <hr class="navbar-divider">
      <div class="columns is-centered mt-section" v-for="c in catalog" v-bind:key="c.id">
        <div class="column is-11 reset-color">
          <h3 class="rs-title-3">{{ c.name }}</h3>
          <div class="columns">
            <div class="column is-2" v-for="p in c.products" v-bind:key="p.id">
              <div class="card">
                <div class="card-image">
                  <figure class="image is-4by3">
                    <img :src="'/img/' + p.image" :alt="p.name">
                  </figure>
                </div>
                <div class="card-content">
                  <div class="content">
                    <a href="/catalog" class="">{{ p.name }}</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <h2 class="main-title">Contactenos</h2>
      <hr class="navbar-divider">
      <div class="columns is-centered mt-section">
        <div class="column is-3">
          <div class="field">
            <p class="control">
              <input name="name" type="text" placeholder="Nombre" class="input">
            </p>
          </div>
          <div class="field">
            <p class="control">
              <input name="subject" type="text" placeholder="Asunto" class="input">
            </p>
          </div>
          <div class="field">
            <p class="control">
              <input name="email" type="email" placeholder="Email" class="input">
            </p>
          </div>
          <div class="field">
            <p class="control">
              <input name="phone" type="number" placeholder="Telefono" class="input">
            </p>
          </div>
          <div class="field">
            <textarea name="message" placeholder="Mensaje..." class="textarea"></textarea>
          </div>
          <div class="field">
            <button class="button is-fullwidth is-warning rs-montserrat rs-semibold">
              ¡COTIZA AHORA!
            </button>
          </div>
        </div>
        <div class="column is-3">
          <iframe id="map" src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d3901.970713500955!2d-77.0520191!3d-12.045536!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8d3897b8dab%3A0x485ba55ce39fedd1!2sIMAWA+PERU!5e0!3m2!1ses-419!2spe!4v1562887771674!5m2!1ses-419!2spe" frameborder="0" allowfullscreen="allowfullscreen" style="border: 0px;"></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        catalog: [
          {
            id: 1,
            name: 'Botas',
            products: [
              { id: 1, name: 'Botas Timberly', image: '/home/product_1.jpg', url: '' },
              { id: 2, name: 'Dickes Medway', image: '/home/product_2.jpg', url: '' },
              { id: 3, name: 'Uvex S2 SRC', image: '/home/product_3.jpg', url: '' },
              { id: 4, name: 'Larmen', image: '/home/product_4.jpg', url: '' },
              { id: 5, name: 'Black Hammer', image: '/home/product_5.jpg', url: '' },
              { id: 6, name: 'Dicker', image: '/home/product_6.jpg', url: '' },
            ]
          },

          {
            id: 2,
            name: 'Protectores',
            products: [
              { id: 7, name: 'Mascara para soldar', image: '/home/product_7.jpg', url: '' },
              { id: 8, name: 'Impermeable', image: '/home/product_8.jpg', url: '' },
              { id: 9, name: 'Casacas', image: '/home/product_9.jpg', url: '' },
              { id: 10, name: 'Cubregafas', image: '/home/product_10.jpg', url: '' },
              { id: 11, name: 'Gafas de seguridad', image: '/home/product_11.jpg', url: '' },
              { id: 12, name: 'Drager X-pect 8321', image: '/home/product_12.jpg', url: '' },
            ]
          },

          {
            id: 3,
            name: 'Otros',
            products: [
              { id: 13, name: 'Arnés anticaída', image: '/home/product_13.jpg', url: '' },
              { id: 14, name: 'Guantes Multiflex', image: '/home/product_14.jpg', url: '' },
              { id: 15, name: 'Guantes Prime', image: '/home/product_15.jpg', url: '' },
              { id: 16, name: 'Gorra Colton', image: '/home/product_16.jpg', url: '' },
              { id: 17, name: 'Casco', image: '/home/product_17.jpg', url: '' },
              { id: 18, name: 'Conos', image: '/home/product_18.jpg', url: '' },
            ]
          }
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  .main-background {
    background-image: url("/img/main-background.svg");
    background-size: cover;
    width: 103vw;
    height: 80vh;
    position: relative;
    top: -70px;
    left: -6px;
  }

  .navbar-divider {
    background-color: #22211e;
  }

  .card {
    box-shadow: 0 0 0;
  }

  .card-content {
    padding-top: 10px;
    padding-left: 0;
    padding-right: 0;
  }
</style>

