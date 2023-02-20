<template>
  <div class="project-detail">
    <div class="project-detail-info-box inbox">
      <div class="project-detail-info">
        <h2>OCEANA LUMINA</h2>
        <div class="project-add-date">
          <div class="project-year">2019</div>
          <div class="project-country">Taipei</div>
        </div>
      </div>
      <div class="project-detail-info-box-line"></div>
      <div class="project-description">
        OMX is a powerful design service carrier. It takes creating unique
        viewpoints and defining forward-looking exhibition curation trends as
        its own responsibility.
      </div>
    </div>
    <div class="project-img-box inbox">
      <div class="project-img">
        <img src="/images/XXTRALAB01.jpg" alt="" class="cover-fit" />
      </div>
      <div class="project-img">
        <img src="/images/XXTRALAB01.jpg" alt="" class="cover-fit" />
      </div>
      <div class="project-img">
        <img src="/images/XXTRALAB01.jpg" alt="" class="cover-fit" />
      </div>
      <div class="project-img">
        <img src="/images/XXTRALAB01.jpg" alt="" class="cover-fit" />
      </div>
    </div>
    <div class="project-tag inbox">
      <span class="project-tag-label">MUSE</span>
      <span class="project-tag-label">SMOOTHY</span>
    </div>
    <div class="swiper inbox">
      <div class="project-detail-slider">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <div class="swiper-slide-box">
              <img
                class="cover-fit"
                src="/images/img_index_banner.jpg"
                alt=""
              />
            </div>
            <div class="project-title">TEA CULTURE</div>
          </div>
          <div class="swiper-slide">
            <div class="swiper-slide-box">
              <img
                class="cover-fit"
                src="/images/img_index_banner02.jpg"
                alt=""
              />
            </div>
            <div class="project-title">TEA CULTURE</div>
          </div>
          <div class="swiper-slide">
            <div class="swiper-slide-box">
              <img
                class="cover-fit"
                src="/images/img_index_banner03.jpg"
                alt=""
              />
            </div>
            <div class="project-title">TEA CULTURE</div>
          </div>
        </div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    // eslint-disable-next-line no-new
    new window.Swiper('.project-detail-slider', {
      slidesPerView: 3,
      loop: true,
      spaceBetween: 20,
      autoplay: {
        delay: 4000,
      },

      breakpoints: {
        768: {
          slidesPerView: 3,
        },
        600: {
          slidesPerView: 2,
        },
        100: {
          slidesPerView: 1,
        },
      },
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
    })
  },
}
</script>
<style>
.project-detail {
  background: #d6dfd9;
}
.project-detail .project-detail-info-box {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 0 60px;
}
@media only screen and (max-width: 600px) {
  .project-detail .project-detail-info-box {
    padding: 0 10px;
  }
}
.project-detail .project-detail-info {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.project-detail .project-detail-info .project-add-date {
  display: flex;
}
.project-detail .project-img-box .project-img {
  margin-bottom: 40px;
}
.project-detail .project-img-box .project-img:nth-last-child(1) {
  margin-bottom: 0;
}
.project-detail .project-tag {
  padding: 50px 0 70px;
  display: flex;
  flex-wrap: nowrap;
}
.project-detail .project-tag span + span {
  margin-left: 20px;
}

.project-detail .project-tag .project-tag-label {
  padding: 10px 20px;
  border-radius: 20px;
  border: 1px solid #000;
}
.project-detail .swiper {
  padding-bottom: 100px;
  overflow: visible;
}
.project-detail .swiper .project-detail-slider {
  overflow: hidden;
}
.project-detail .swiper .swiper-slide .project-title {
  padding: 10px;
  background: #6d7270;
  color: #fff;
}
.project-detail .swiper .swiper-slide .swiper-slide-box {
  height: 150px;
}

.project-detail .swiper .swiper-button-next,
.project-detail .swiper .swiper-button-prev {
  color: var(--color-secondary);
  top: 80%;
  border-radius: 50%;
  border: 1px solid #000;
  width: 50px;
  height: 50px;
}
.project-detail .swiper .swiper-button-next {
  right: 2%;
}
.project-detail .swiper .swiper-button-next:after {
  font-size: 24px;
}
.project-detail .swiper .swiper-button-prev {
  left: 80%;
}
.project-detail .swiper .swiper-button-prev:after {
  font-size: 24px;
}
</style>
