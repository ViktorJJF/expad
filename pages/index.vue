<template>
  <div>
    <!-- header -->
    <header class="main-header">
      <div class="background-overlay text-white py-5">
        <b-container fluid class="text-light text-center">
          <b-row>
            <b-col
              cols="12"
              md="6"
              class="text-center justify-content-center align-self-center"
            >
              <h1>Este es un titulo</h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Non,
                eum?
              </p>
              <b-button variant="outline-light">Leer más</b-button>
            </b-col>
            <b-col cols="12" md="6" class="text-center">
              <img
                src="/images/product.jpg"
                alt="Imagen del producto"
                class="img-fluid d-none d-sm-block"
              />
            </b-col>
          </b-row>
        </b-container>
      </div>
    </header>
    <!-- NEWSLETTER -->
    <section class="bg-dark text-white py-5">
      <b-container fluid class="custom-width">
        <b-row>
          <b-col sm>
            <b-form-input
              size="lg"
              v-model="form.email"
              type="email"
              required
              placeholder="Ingrese su nombre"
            ></b-form-input>
          </b-col>
          <b-col sm>
            <b-form-input
              size="lg"
              v-model="form.email"
              type="email"
              required
              placeholder="Ingrese su email"
            ></b-form-input>
          </b-col>
          <b-col sm>
            <b-button block size="lg" variant="success">Suscribirse</b-button>
          </b-col>
        </b-row>
      </b-container>
    </section>
    <!-- FEATURES -->
    <section class="py-5">
      <b-container fluid>
        <b-row>
          <b-col sm
            ><b-card
              border-variant="primary"
              title="Caracteristica 1"
              align="center"
            >
              <b-card-text
                >Lorem ipsum dolor sit amet, consectetur adipiscing
                elit.</b-card-text
              >
            </b-card>
          </b-col>
          <b-col sm
            ><b-card
              border-variant="primary"
              bg-variant="primary"
              text-variant="white"
              title="Caracteristica 1"
              align="center"
            >
              <b-card-text
                >Lorem ipsum dolor sit amet, consectetur adipiscing
                elit.</b-card-text
              >
            </b-card>
          </b-col>
          <b-col sm
            ><b-card title="Card Title" class="mb-2">
              <b-card-text>
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </b-card-text>
            </b-card>
          </b-col>
          <b-col sm
            ><b-card
              title="Card Title"
              bg-variant="primary"
              text-variant="white"
              class="mb-2"
            >
              <b-card-text>
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </b-card-text>
            </b-card>
          </b-col>
        </b-row>
      </b-container>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: { email: '' }
    }
  }
}
</script>

<style>
.container-fluid {
  width: 80%;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
