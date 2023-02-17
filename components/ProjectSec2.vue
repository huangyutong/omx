<template>
  <div class="product_slider">
    <div class="inbox_banner">
      <div class="swiper banner_slider">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <div class="banner_pic">
              <img class="cover-fit" src="/images/img_banner_01.jpg" alt="" />
            </div>
          </div>
          <div class="swiper-slide">
            <div class="banner_pic">
              <img class="cover-fit" src="/images/img_banner_01.jpg" alt="" />
            </div>
          </div>
          <div class="swiper-slide">
            <div class="banner_pic">
              <img class="cover-fit" src="/images/img_banner_01.jpg" alt="" />
            </div>
          </div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    window.jQuery(document).ready(function () {
      // Menu
      window.jQuery('.swiper-pagination-bullet').click(function () {
        window.jQuery(this).addClass('swiper-pagination-bullet-active')
        window
          .jQuery('.swiper-pagination-bullet')
          .siblings()
          .removeClass('swiper-pagination-bullet-active')
      })
    })
    // eslint-disable-next-line no-new
    new window.Swiper('.banner_slider', {
      loop: true,
      spaceBetween: 30,
      autoplay: {
        delay: 6000,
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
    })
  },
}
</script>
<style>
.product_slider {
}
.product_slider .swiper {
  height: calc(100vh - var(--navbar-height));
  padding: 30px 0;
  border-radius: 20px;
}
.product_slider .swiper-wrapper {
  border-radius: 20px;
}
.product_slider .swiper-wrapper .swiper-slide {
  border: 2px solid #b6a999;
  border-radius: 20px;
  overflow: hidden;
}
.product_slider .swiper-wrapper .swiper-slide .banner_pic {
  height: 100%;
  border-radius: 20px;
}
.product_slider .swiper-pagination {
  margin: 0 0 30px 20px;
  text-align: left;
}
.product_slider .swiper-pagination .swiper-pagination-bullet {
  margin: 0 15px;
  width: 12px;
  height: 12px;
  background: #fff;
  opacity: 1;
}
.product_slider .swiper-pagination .swiper-pagination-bullet:hover {
  background: #d9c2b6 !important;
}
.product_slider .swiper-pagination .swiper-pagination-bullet-active {
  background: #d9c2b6;
  position: relative;
}
.product_slider .swiper-pagination .swiper-pagination-bullet-active::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 30px;
  height: 30px;
  border-radius: 50%;
  border: 1px solid #d9c2b6 !important;
}
</style>
