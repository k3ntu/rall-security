<template>
  <div>
    <section class="hero is-medium is-black has-background">
      <img src="/img/banner.jpg" alt="Fill Murray" class="hero-background is-transparent">
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="columns is-centered">
            <div class="column is-half">
              <h1 class="title rs-title">
                ¿Qué es rall security?
              </h1>
            </div>
          </div>

          <div class="columns is-centered">
            <div class="column is-6">
              <h2 class="subtitle rs-subtitle">
                Somos la empresa dedicada a la venta de productos de seguridad. Si trabajas en una construcción o un agente de seguridad tenemos productos a tu medida.
              </h2>
            </div>
          </div>
        </div>
      </div>
    </section>

    <div class="container my-section">
      <h2 class="main-title mb-section">Principios</h2>
      <div class="tile is-ancestor is-centered has-text-centered">
        <div class="tile is-vertical is-12">
          <div class="tile">
            <div class="tile is-parent">
              <article class="tile is-child">
                <figure>
                  <img src="./../assets/icons/shield.svg" alt="">
                </figure>
                <p class="title">Seguridad</p>
                <p class="subtitle">Nuestros artículos pasan por rigurosas pruebas antes de llegar a sus manos.</p>
              </article>
            </div>

            <div class="tile is-parent">
              <article class="tile is-child">
                <figure>
                  <img src="./../assets/icons/hourglass.svg" alt="">
                </figure>
                <p class="title">Resistencia</p>
                <p class="subtitle">Tener la seguridad de que nada falle. Es solo un símbolo de nuestro sello.</p>
              </article>
            </div>

            <div class="tile is-parent">
              <article class="tile is-child">
                <figure style="padding-bottom: 14px;">
                  <img src="./../assets/icons/like.svg" alt="">
                </figure>
                <p class="title">Sentir</p>
                <p class="subtitle">Llevamos más de 10 años en el mercado, por lo que siempre pensamos en usted.</p>
              </article>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import "./../scss/variables";

  .rs-title {
    font-family: $roboto;
    font-weight:900;
    font-size: $rs-title;
  }
  .rs-subtitle {
    font-family: $montserrat;
    font-weight:300
  }

  .hero.has-background {
    position:relative;
    overflow:hidden
  }
  .hero-background {
    position:absolute;
    -o-object-fit:cover;
    object-fit:cover;
    -o-object-position:center center;
    object-position:center center;
    width:100%;
    height:100%
  }

  .hero-background.is-transparent {
    opacity:.3
  }
</style>
