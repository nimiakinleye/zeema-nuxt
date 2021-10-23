<template>
  <div>
    <AppHeader />
    <Banner />
    <About />
    <Rates />
    <Benefits />
    <Subscribe />
    <AppFooter />
    <div @click="toTop" :class="{show: scroll, hide:!scroll }" class="scroll_up">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256">
        <rect width="256" height="256" fill="none" />
        <circle
          cx="128"
          cy="128"
          r="96"
          fill="none"
          stroke="#00803d"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="24"
        />
        <polyline
          fill="none"
          stroke="#00803d"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="24"
          points="94.059 121.941 128 88 161.941 121.941"
        />
        <line
          x1="128"
          x2="128"
          y1="168"
          y2="88"
          fill="none"
          stroke="#00803d"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="24"
        />
      </svg>
    </div>
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

  data() {
    return {
      scroll: false
    }
  },

  methods: {
    onScroll() {
      if(window.pageYOffset > 50) {
        this.scroll = true
      } else {
        this.scroll = false
      }
    },
    toTop() {
      document.body.scrollTop = 0 // For Safari
      document.documentElement.scrollTop = 0 // For Chrome
    }
  },

  beforeMount() {
    window.addEventListener('scroll', this.onScroll)
  }
}
</script>

<style scoped>
.scroll_up {
  width: 50px;
  position: fixed;
  bottom: 30px;
  right: 40px;
  transition: 1000ms;
  cursor: pointer;
}

.scroll_up svg {
  border-radius: 100%;
  background-color: rgba(255, 255, 255, 0.2);
}

.hide {
  transform: translateY(1000%);
}
.show {
  transform: translateY(0);
}
</style>
