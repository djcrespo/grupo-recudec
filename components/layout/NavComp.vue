<template>
  <b-navbar
    :spaced="true"
    type="is-white"
  >
    <template #brand>
      <b-navbar-item>
        <b-image
          :src="require('@/assets/img/logo.png')"
        ></b-image>
      </b-navbar-item>
    </template>

    <template #end>
      <b-navbar-item href="#inicio">Inicio</b-navbar-item>
      <b-navbar-item href="#nosotros">Nuestra empresa</b-navbar-item>
      <b-navbar-item href="#productos">Productos</b-navbar-item>
      <b-navbar-item href="#servicios">Servicios</b-navbar-item>
      <!--<b-navbar-item href="#portafolio">Portafolio</b-navbar-item>-->
      <b-navbar-item href="#contacto">Contacto</b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
export default {
  name: 'NavBarComponent'
}
</script>

<style>
</style>
