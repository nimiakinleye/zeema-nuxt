<template>
  <section class="container">
    <div id="rates">
      <div data-aos="flip-up" class="rates">
        <div class="rate">
          <div class="img">
            <img src="~/assets/rates/savings.png" alt="" />
          </div>
          <div>
            <h3>Savings</h3>
            <p>up to 0.50% APY</p>
          </div>
        </div>
        <div class="rate">
          <div class="img">
            <img src="~/assets/rates/certificates.png" alt="" />
          </div>
          <div>
            <h3>Certificates</h3>
            <p>up to 3.00% APY</p>
          </div>
        </div>
        <div class="rate">
          <div class="img">
            <img src="~/assets/rates/credit-card.png" alt="" />
          </div>
          <div>
            <h3>Credit card</h3>
            <p>as low as 5.99% APY</p>
          </div>
        </div>
      </div>
      <div data-aos-delay="300" data-aos="fade-up" class="more">
        <nuxt-link to="#">
          <span>View more rates</span>
          <span>
            <svg width="10" height="5" viewBox="0 0 16 8" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M7.82483 1.06759L11.6667 3.35043L9.33102e-08 3.35043L6.54855e-08 4.73691L11.6667 4.73691L7.82483 7.01976L9.4745 8L14.483 5.02391C14.9204 4.76391 15.1662 4.41132 15.1662 4.04367C15.1662 3.67603 14.9204 3.32343 14.483 3.06343L9.4745 0.0873414L7.82483 1.06759Z"
                fill="#00803D" />
            </svg>
          </span>
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style>
</style>