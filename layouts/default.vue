<template>
  <div class="color-back">
    <nav-comp></nav-comp>
    <section class="main-content columns">
      <div class="container column">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style>
.color-back {
  width: 100%;
  background-color: #F7B84D;
}
</style>
