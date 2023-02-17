<template>
  <div class="banner_box">
    <h1 class="banner_title animate__animated animate__fadeIn">WE ARE OMX</h1>
    <div class="banner_next_btn">
      <div id="circle" class="btn_circle">
        <a href="#sec2" class="scroll">
          <i class="fa-solid fa-arrow-down"></i
        ></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
.banner_box {
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
.animate__animated.animate__fadeIn {
  --animate-delay: 3s;
  --animate-duration: 4s;
}
.banner_box:after {
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
}
.banner_title {
  z-index: 5;
  font-weight: 500;
  font-size: 3em;
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translateX(-50%);
}
.svg-inline--fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 2.5em;
  color: #fff;
}
</style>
