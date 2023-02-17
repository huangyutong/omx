<template>
  <div class="about_banner_box">
    <div class="inbox banner_content">
      <p></p>
      <div class="text">
        <h1 class="banner_title">
          OMX is the signatificant combination group with Moxie and Xxtralab.
        </h1>
        <p>
          we combined our service to improve the best for our customer.The
          standard chunk of torem Ipsum used since the 1500s is reproduced below
          for those interested .Sections 1,10,32 and 1.10.33 from “deFinibus
          Bonoruum et Malorum”
        </p>
      </div>
      <div class="banner_next_btn">
        <div class="btn_circle">
          <a href=""><i class="fa-solid fa-plus"></i></a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    window.jQuery('.btn_circle').click(function () {})
  },
}
</script>
<style scoped>
.about_banner_box {
  height: 100vh;
  background-image: url('/images/img_index_banner.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  color: #f2f2f2;
  display: flex;
  /* align-items: center; */
  /* justify-content: space-around; */
  /* flex-direction: column; */
  position: relative;
}
.about_banner_box:after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background: rgba(0, 0, 0, 0.4);
  z-index: 1;
}

.banner_next_btn {
  z-index: 5;
  position: relative;
}
.about_banner_box .btn_circle {
  border-radius: 50%;
  border: 2px solid #ffffff;
  width: 80px;
  height: 80px;
  position: relative;
  cursor: pointer;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  z-index: 100;
  bottom: 20px;
}
.about_banner_box .banner_title {
  max-width: 600px;
  z-index: 5;
  font-weight: 500;
  font-size: 3em;
  line-height: 60px;
}
.about_banner_box h1.banner_title {
  margin-top: 0;
}
.about_banner_box .banner_content {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: relative;
  z-index: 10;
  text-align: left;
}
.about_banner_box .banner_content p {
  max-width: 800px;
}
.about_banner_box .btn_circle:before {
  content: 'Read More';
  position: absolute;
  top: -50px;
  left: 50%;
  white-space: nowrap;
  transform: translateX(-50%);
}
.about_banner_box .btn_circle p {
  white-space: nowrap;
  position: absolute;
}
.about_banner_box .btn_circle a {
  color: #fff;
}
.fa-plus {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 2.5em;
}
</style>
