<template>
  <section class="section">
    <nav aria-label="breadcrumbs" class="breadcrumb">
      <ul>
        <li>
          <a href="#">Construcción</a>
        </li>
        <li>
          <a href="#">Protectores</a>
        </li>
        <li class="is-active">
          <a href="#" aria-current="page">Botas</a>
        </li>
      </ul>
    </nav>

    <div class="container is-fluid my-section-1">
      <h1 class="main-title">Botas</h1>
      <div class="columns">
        <div class="column is-3">
          <div class="card">
            <div class="card-content">
              <div>
                <p class="subtitle">Talla</p>
                <ul class="rs-bullet-list">
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">25</label>
                  </li>
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">26</label>
                  </li>
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">27</label>
                  </li>
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">28</label>
                  </li>
                </ul>
              </div>
              <hr class="navbar-divider">
              <div>
                <p class="subtitle">Sexo</p>
                <ul class="rs-bullet-list">
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">F</label>
                  </li>
                  <li>
                    <label class="checkbox"><input type="checkbox">M</label>
                  </li>
                </ul>
              </div>
              <hr class="navbar-divider">
              <div>
                <p class="subtitle">Marca</p>
                <ul class="rs-bullet-list">
                  <li><label class="checkbox">
                    <input type="checkbox">Cat</label>
                  </li>
                  <li><label class="checkbox">
                    <input type="checkbox">Wallom</label>
                  </li>
                  <li>
                    <label class="checkbox">
                      <input type="checkbox">Timberly
                    </label>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>

        <div class="column is-9">
          <div class="columns is-multiline">
            <div class="column is-3" v-for="p in products" v-bind:key="p.id">
              <div class="card rs-box-none">
                <div class="card-image">
                  <figure class="image is-4by3">
                    <img :src="'/img/' + p.image" :alt="p.name">
                  </figure>
                </div>
                <div class="card-content rs-content-none-padding">
                  <div class="content">
                    <p class="rs-card-title">{{ p.name }}</p>
                    <p class="rs-card-subtitle">{{ p.marca }}</p>
                    <p class="rs-card-price rs-yellow-dark-1">S/. {{ p.price }}</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        products: [
          { id: 1, name: 'Botas Timberly', marca: 'Timberly', price: 459.00, image: '/home/product_1.jpg', url: '' },
          { id: 2, name: 'Dickes Medway', marca: 'Timberly', price: 459.00, image: '/home/product_2.jpg', url: '' },
          { id: 3, name: 'Uvex S2 SRC', marca: 'Timberly', price: 459.00, image: '/home/product_3.jpg', url: '' },
          { id: 4, name: 'Larmen', marca: 'Timberly', price: 459.00, image: '/home/product_4.jpg', url: '' },
          { id: 5, name: 'Black Hammer', marca: 'Timberly', price: 459.00, image: '/home/product_5.jpg', url: '' },
          { id: 6, name: 'Dicker', marca: 'Timberly', price: 459.00, image: '/home/product_6.jpg', url: '' },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "./../scss/variables";

  .rs-bullet-list {
    padding-left: 20px;
  }

  .content p {
    margin-bottom: 0;
  }

  .rs-card-title {
    font-family: $roboto;
    font-weight: 600;
    font-size: $rs-quote;
    color: $rs-black;
  }

  .rs-card-subtitle {
    font-weight: 300;
    color: $rs-black;
  }

  .rs-card-subtitle, .rs-card-price {
    font-family: $montserrat;
    font-size: $rs-normal;
  }
</style>