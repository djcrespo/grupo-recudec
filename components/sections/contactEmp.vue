<template>
  <div id="contacto" class="container m-4">
    <div class="card">
      <div class="card-content">
        <p class="title has-text-centered">Contacto</p>
        <section class="section">
          <div class="columns is-flex is-justify-content-center">
            <div class="column is-5">
              <form>
                <b-field label="Nombre">
                  <b-input v-model="form.name"></b-input>
                </b-field>
                <b-field label="Email">
                  <b-input v-model="form.email" type="email"></b-input>
                </b-field>
                <b-field label="Teléfono">
                  <b-input v-model="form.phone" type="number"></b-input>
                </b-field>
                <b-field label="Empresa">
                  <b-input v-model="form.empresa"></b-input>
                </b-field>
                <b-field label="Mensaje">
                  <b-input
                    v-model="form.message"
                    type="texarea"
                    maxlength="200"
                  ></b-input>
                </b-field>
              </form>
            </div>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactComponent',
  data () {
    return {
      form: {}
    }
  },
  methods: {
    submit () {}
  }
}
</script>
