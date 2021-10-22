<template>
  <header class="container" id="header">
    <div id="lg_header">
      <div id="logo_nav">
        <nuxt-link to="#">
          <img class="logo" src="~/assets/logo.svg" alt="" />
        </nuxt-link>
        <div class="navlinks">
          <nuxt-link to="/" class="navlink">Home</nuxt-link>
          <nuxt-link to="#" class="navlink">Contact</nuxt-link>
          <nuxt-link to="#" class="navlink">Services</nuxt-link>
          <nuxt-link to="#" class="navlink">Resources</nuxt-link>
          <nuxt-link to="#" class="navlink">Membership</nuxt-link>
        </div>
      </div>
      <div>
        <nuxt-link to="#" class="navlink login">Login</nuxt-link>
        <nuxt-link to="#" class="navlink button">Apply now</nuxt-link>
      </div>
    </div>
  </header>
</template>

<script>
export default {}
</script>

<style>
</style>