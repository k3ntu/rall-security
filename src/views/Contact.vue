<template>
  <section class="section rs-body-white">
    <div class="container">
      <h1 class="title rs-title has-text-centered">Tienes un pedido más grande.<br>Cotiza ahora.</h1>
      <div class="columns is-centered">
        <div class="column is-half">
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
      </div>
    </div>
  </section>
</template>