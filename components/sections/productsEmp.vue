<template>
  <div id="productos" class="container m-4">
    <div class="card">
      <div class="card-content">
        <div class="columns">
          <div class="column">
            <p class="title has-text-centered">
              Los mejores productos para tí.
            </p>
            <section class="section">
              <b-carousel animated="fade" :arrow="false" :indicator="false">
                <b-carousel-item v-for="(product, i) in products" :key="i">
                  <b-image :src="product.img"></b-image>
                </b-carousel-item>
              </b-carousel>
            </section>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductsComponent',
  data () {
    return {
      products: [
        {
          img: require('@/assets/img/products/cemix.png')
        },
        {
          img: require('@/assets/img/products/sika.png')
        },
        {
          img: require('@/assets/img/products/al-koat.png')
        },
        {
          img: require('@/assets/img/products/fibercon.jpeg')
        },
        {
          img: require('@/assets/img/products/nervion.jpeg')
        },
        {
          img: require('@/assets/img/products/proconsa.jpeg')
        }
      ]
    }
  }
}
</script>
