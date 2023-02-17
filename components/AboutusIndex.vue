<template>
  <div class="about_box" id="sec2">
    <h1 class="about_title">
      AT OMX, <br />
      WE BRING PEOPLE <br />TOGETHER.
    </h1>
    <div class="banner_content">
      Whether at a concert,a flagship store or across an urban square,
    </div>
   
    <div id="circle" class="btn_circle">
      <a href="#exhibition" class="scroll">
        <i class="fa-solid fa-arrow-down"></i>
      </a>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
.about_box {
  height: 100vh;
  background: #d6dfd9;
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  position: relative;
}

.about_box .btn_circle {
  border: 2px solid #000;
}
.banner_content,
.about_box .btn_circle,
.about_box .about_us_btn,
.about_title {
  z-index: 5;
}

.about_title {
  font-weight: 500;
  z-index: 5;
  font-size: 3em;
  line-height: 50px;
}
.about_box .about_us_btn a {
  padding: 10px 25px;
  border: 1px solid #000;
  border-radius: 50px;
  display: block;
  margin: 30px 0px;
}
</style>
