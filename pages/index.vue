<template>
  <div>
    <AppHeader />
    <Banner />
    <About />
    <Rates />
    <Benefits />
    <Subscribe />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
import Banner from '~/components/Banner.vue'
import About from '~/components/About.vue'
import Rates from '~/components/Rates.vue'
import Benefits from '~/components/Benefits.vue'
import Subscribe from '~/components/Subscribe.vue'
import AppFooter from '~/components/AppFooter.vue'
export default {
  components: {
    AppHeader,
    Banner,
    About,
    Rates,
    Benefits,
    Subscribe,
    AppFooter,
  },
}
</script>
