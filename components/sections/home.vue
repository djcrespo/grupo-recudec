<template>
  <div id="inicio" class="container m-4">
    <div class="card">
      <div class="card-content m-4">
        <p class="title">
          Recubrimiento Decorativo – Empresa Especializada en Impermeabilizantes
          del Sureste de México.
        </p>
        <br />
        <p class="subtitle has-text-justified">
          Ofrecemos nuestros servicios al sector público y privado, para brindar
          lo mejor de nuestros productos, en especial la venta y aplicación de
          impermeabilizantes. Nuestros servicios están plenamente garantizados,
          ya que trabajamos con las mejores marcas. Lo mejor en
          impermeabilizantes en el sureste al mejor precio, solo con nosotros.
        </p>
        <section class="section">
          <div v-animate-css="animationImage" class="card">
            <div class="card-image">
              <b-image :src="require('@/assets/img/cover1.png')"></b-image>
            </div>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeComponent',
  data () {
    return {
      animationImage: {
        classes: 'fadeInUp',
        delay: 1000,
        duration: 1500
      }
    }
  }
}
</script>
