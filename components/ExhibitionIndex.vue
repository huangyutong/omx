<template>
  <section id="exhibition" class="index_item_box">
    <div class="inbox index_item_box_content">
      <Tab />
      <div class="exhibition-content">
        OMX is a powerful design service carrier. It takes creating unique
        viewpoints and defining forward-looking exhibition curation trends as
        its own responsibility.
      </div>
    </div>
    <div class="swiper">
      <div class="home_exhibition_slider">
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
    new window.Swiper('.home_exhibition_slider', {
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
<style>
#exhibition {
  position: relative;
}

.index_item_box {
  height: 100vh;
  /* text-align: center;
  color: #f2f2f2;
  display: flex;
  align-items: center;
  flex-direction: column;
  position: relative; */
}

#exhibition .inbox {
  position: absolute;
  top: 46px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 9;
}
#exhibition .exhibition-content {
  margin-top: 170px;
  color: #fff;
  width: 70%;
  max-width: 750px;
}
.index_item_box .swiper-wrapper {
  height: 100vh;
}
.index_item_box .swiper .swiper-slider {
  height: auto;
}
</style>
