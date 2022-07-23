<template>
  <div id="servicios" class="container m-4">
    <div class="card">
      <div class="card-content">
      <div class="columns">
        <div class="column">
          <p class="title has-text-centered">
            Servicios
          </p>
        </div>
      </div>
        <div class="columns">
          <div class="column">
            <section class="section">
              <b-carousel animated="fade" :arrow="false" :indicator="false">
                <b-carousel-item v-for="(item, i) in items" :key="i">
                  <b-image :src="item.img"></b-image>
                </b-carousel-item>
              </b-carousel>
            </section>
          </div>
          <div class="column is-5">
            <p class="subtitle has-text-justified my-6">
              Recudec ofrece una amplia variedad de productos, siempre
              respaldado por el profesionalismo de nuestros aplicadores.
            </p>
            <p class="subtitle has-text-justified my-6">
              Ofrecemos las mejores marcas en impermeabilizantes Sika, Al Koat,
              Proconsa.
            </p>
            <p class="subtitle has-text-justified my-6">
              Servimos al sector público y privado. Tenemos una amplia cartera
              de clientes que han confiado en nuestros servicios.
            </p>
            <p class="subtitle has-text-justified my-6">
              Cuidamos su patrimonio y su inversión, con nuestro equipo de
              trabajo altamente capacitado.
            </p>
            <p class="subtitle has-text-justified my-6">
              Contáctenos y uno de nuestros asesores le dará la información,
              sobre el producto más adecuado a sus necesidades.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ServicesComponent',
  data () {
    return {
      items: [
        {
          img: require('@/assets/img/img4.png')
        },
        {
          img: require('@/assets/img/img5.png')
        },
        {
          img: require('@/assets/img/img6.png')
        }
      ]
    }
  }
}
</script>
