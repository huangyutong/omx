<template>
  <section id="interection" class="index_item_box">
    <div class="swiper">
      <div class="home_interection_slider">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img class="cover-fit" src="/images/img_index_banner.jpg" alt="" />
          </div>
          <div class="swiper-slide">
            <img
              class="cover-fit"
              src="/images/img_index_banner02.jpg"
              alt=""
            />
          </div>
          <div class="swiper-slide">
            <img
              class="cover-fit"
              src="/images/img_index_banner03.jpg"
              alt=""
            />
          </div>
        </div>
      </div>
      <div class="home-application-slider-pagination"></div>
    </div>
  </section>
</template>
<script>
export default {
  mounted() {
    // eslint-disable-next-line no-new
    new window.Swiper('.home_interection_slider', {
      slidesPerView: 1,
      loop: true,
      spaceBetween: 30,
      autoplay: {
        delay: 6000,
      },
      breakpoints: {
        1220: {
          slidesPerView: 1,
        },
      },
    })
  },
}
</script>
