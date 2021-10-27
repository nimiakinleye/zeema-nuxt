<template>
  <section class="container">
    <div id="banner">
      <div data-aos="flip-left" id="banner_text">
        <h1 class="title">
          Best <br />Credit<br />
          Solution
        </h1>
        <p class="caption">US based credit union for American immigrants.</p>
        <button>
          <p>Apply now</p>
          <svg
            width="10"
            height="10"
            viewBox="0 0 14 14"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g clip-path="url(#clip0)">
              <path
                d="M12.9039 5.76275L7.14345 0L6.31862 0.827167L12.079 6.58758C12.1884 6.69697 12.2498 6.84532 12.2498 7C12.2498 7.15468 12.1884 7.30303 12.079 7.41242L6.31104 13.1833L7.13587 14.0082L12.9039 8.24017C13.2319 7.91199 13.4162 7.46695 13.4162 7.00292C13.4162 6.53888 13.2319 6.09384 12.9039 5.76567V5.76275Z"
                fill="#00803D"
              />
              <path
                d="M7.89542 6.58758L1.3195 0.0110836L0.494088 0.835917L6.65817 7L0.487671 13.1705L1.3125 13.9959L7.89542 7.41242C8.00478 7.30303 8.06621 7.15468 8.06621 7C8.06621 6.84532 8.00478 6.69697 7.89542 6.58758Z"
                fill="#00803D"
              />
            </g>
            <defs>
              <clipPath id="clip0">
                <rect width="14" height="14" fill="white" />
              </clipPath>
            </defs>
          </svg>
        </button>
        <p class="tagline">Member-owned. Banking on the American Dream</p>
      </div>
      <div id="banner_img">
        <div data-aos="fade-left" id="svg_1">
          <div class="benefits_svg">
            <div class="duplicate"></div>
            <div class="duplicate_2"></div>
            <img src="~/assets/benefits/low_price.svg" alt="" />
            <span>Lower fees</span>
          </div>
        </div>
        <div data-aos-delay="300" data-aos="fade-right" id="svg_2">
          <div class="benefits_svg">
            <div class="duplicate"></div>
            <div class="duplicate_2"></div>
            <img src="~/assets/benefits/credit_asst.svg" alt="" />
            <span>Credit Assistance</span>
          </div>
        </div>
        <div data-aos-delay="600" data-aos="fade-left" id="svg_3">
          <div class="benefits_svg">
            <div class="duplicate"></div>
            <div class="duplicate_2"></div>
            <img src="~/assets/benefits/savings.svg" alt="" />
            <span>Increased savings</span>
          </div>
        </div>
        <div data-aos-delay="900" data-aos="fade-right" id="svg_4">
          <div class="benefits_svg">
            <div class="duplicate"></div>
            <div class="duplicate_2"></div>
            <img src="~/assets/benefits/rate.svg" alt="" />
            <span>Lower loan rates</span>
          </div>
        </div>
        <div data-aos-delay="1200" data-aos="fade-left" id="svg_5">
          <div class="benefits_svg">
            <div class="duplicate"></div>
            <div class="duplicate_2"></div>
            <img src="~/assets/benefits/voting.svg" alt="" />
            <span>Voting rights</span>
          </div>
        </div>
        <img data-aos="flip-right" src="~/assets/Zema-banner.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
import aosMixin from '~/mixins/aos'
export default {
  mixins: [aosMixin],
}
</script>

<style>
</style>