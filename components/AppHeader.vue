<template>
  <header class="container" id="header">
    <div id="lg_header">
      <div id="logo_nav">
        <a href="#">
          <img class="logo" src="~/assets/logo.svg" alt="" />
        </a>
        <nav class="navlinks">
          <a href="/" class="navlink">Home</a>
          <a href="#subscribe" class="navlink">Contact</a>
          <a href="#benefits" class="navlink">Services</a>
          <a href="#rates" class="navlink">Resources</a>
          <a href="#about" class="navlink">Membership</a>
        </nav>
      </div>
      <div>
        <a href="#" class="navlink login">Login</a>
        <a href="#subscribe" class="navlink button">Apply now</a>
      </div>
    </div>

    <div id="mobile_header">
      <div class="logo_nav">
        <a href="/"
          ><img src="~/assets/logo.svg" alt="" class="logo"
        /></a>
        <div v-on:click="toggleNav" v-html="navSvg"></div>
      </div>
      <nav v-if="show_nav">
        <!-- <a href="#">Home</a>
        <a href="#">Home</a>
        <a href="#">Home</a>
        <a href="#">Home</a>
        <a href="#">Home</a> -->
      </nav>
    </div>
  </header>
</template>

<script>
const menu_svg = `<svg
            viewBox="0 0 512 512"
            style="enable-background: new 0 0 512 512"
            xml:space="preserve"
          >
            <g transform="translate(1 1)">
              <g>
                <g>
                  <path
                    d="M255-1C113.618-1-1,113.618-1,255s114.618,256,256,256s256-114.618,256-256S396.382-1,255-1z M255,468.333     c-117.818,0-213.333-95.515-213.333-213.333S137.182,41.667,255,41.667S468.333,137.182,468.333,255S372.818,468.333,255,468.333     z"
                  />
                  <path
                    d="M361.667,148.333H148.333c-11.782,0-21.333,9.551-21.333,21.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,157.885,373.449,148.333,361.667,148.333z"
                  />
                  <path
                    d="M361.667,233.667H148.333C136.551,233.667,127,243.218,127,255s9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333S373.449,233.667,361.667,233.667z"
                  />
                  <path
                    d="M361.667,319H148.333C136.551,319,127,328.551,127,340.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,328.551,373.449,319,361.667,319z"
                  />
                </g>
              </g>
            </g>
          </svg>`
export default {
  data() {
    return {
      navSvg: menu_svg,
      show_nav: false,
    }
  },

  methods: {
    toggleNav() {
      if (this.show_nav === false) {
        this.show_nav = true
        this.navSvg = `<svg
            class="w-8 fill-current my-color"
            viewBox="0 0 340.8 340.8"
            style="enable-background: new 0 0 340.8 340.8"
            xml:space="preserve"
          >
            <g>
              <g>
                <path
                  d="M170.4,0C76.4,0,0,76.4,0,170.4s76.4,170.4,170.4,170.4s170.4-76.4,170.4-170.4S264.4,0,170.4,0z M170.4,323.6    c-84.4,0-153.2-68.8-153.2-153.2S86,17.2,170.4,17.2S323.6,86,323.6,170.4S254.8,323.6,170.4,323.6z"
                />
              </g>
            </g>
            <g>
              <g>
                <path
                  d="M182.4,169.6l50-50c3.2-3.2,3.2-8.8,0-12c-3.2-3.2-8.8-3.2-12,0l-50,50l-50-50c-3.2-3.2-8.8-3.2-12,0    c-3.2,3.2-3.2,8.8,0,12l50,50l-50,49.6c-3.2,3.2-3.2,8.8,0,12c1.6,1.6,4,2.4,6,2.4s4.4-0.8,6-2.4l50-50l50,50c1.6,1.6,4,2.4,6,2.4    s4.4-0.8,6-2.4c3.2-3.2,3.2-8.8,0-12L182.4,169.6z"
                />
              </g>
            </g>
          </svg>`
      } else {
        this.show_nav = false
        this.navSvg = menu_svg
      }
    },
  },
}
</script>

<style>
@keyframes slide {
  0% {
    transform: translateY(-1000%);
  }
  100% {
    transform: translateY(0);
  }
}
</style>