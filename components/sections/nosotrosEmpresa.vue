<template>
  <div id="nosotros" class="container m-4">
    <div class="card">
      <div class="card-content">
        <p class="title">
          Nuestra Empresa
        </p>
        <br />
        <p class="subtitle has-text-justified mx-3">
          Recubrimiento Decorativo, empresa especializada en impermeabilizantes
          y aditivos, que contribuye a sus soluciones en construcción y
          mantenimiento, con el objetivo de satisfacer las necesidades de los
          clientes, con productos de la mejor calidad para la industria.
        </p>
        <p class="subtitle has-text-justified mx-3">
          Gracias a nuestra extensa línea de productos le ofrecemos, calidad
          garantizada en aditivos, selladores, impermeabilizantes, morteros,
          recubrimientos y pisos; pinturas epóxicas , así como adhesivos
          epóxicos y anclajes.
        </p>
        <p class="subtitle has-text-justified mx-3">
          Contamos con un experimentado equipo de trabajo, que le asesorará en
          el uso de nuestros productos.
        </p>
        <p class="subtitle has-text-justified mx-3">
          Las marcas líderes del mercado, impermeabilizantes Sika , AlKoat y
          Proconsa nos respaldan. En Recudec encontrará todo lo que busca en
          impermeabilizantes, aditivos para concreto, selladores, rollos
          prefabricados para impermeabilizar, contribuyendo a sus soluciones en
          construcción y mantenimiento.
        </p>
        <section class="section mg-small">
          <b-carousel
            animated="fade"
            :arrow="false"
            :indicator="false"
          >
            <b-carousel-item v-for="(item, i) in items" :key="i">
              <b-image :src="item.img"></b-image>
            </b-carousel-item>
          </b-carousel>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NosotrosComponent',
  data () {
    return {
      items: [
        {
          img: require('@/assets/img/img1.png')
        },
        {
          img: require('@/assets/img/img2.png')
        },
        {
          img: require('@/assets/img/img3.png')
        }
      ]
    }
  }
}
</script>
