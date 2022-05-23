<template>
  <div class="contact_index_box">
    <div class="plus">
      <i class="fa-solid fa-plus"></i>
    </div>

    <div class="inbox layout">
      <div class="contact_index">
        <h1 class="title">
          Contact<br />
          Us
        </h1>
        <div class="sub_title">With new business inquiry</div>
      </div>

      <div class="contact_bottom">
        <div class="icon_box">
          <a href="" class="icon fb">
            <i class="fa-brands fa-facebook-f"></i>
          </a>
          <a href="" class="icon yt">
            <i class="fa-brands fa-youtube"></i>
          </a>
          <a href="" class="icon linkedin">
            <i class="fa-brands fa-twitter"></i>
          </a>
        </div>
        <hr />
        <div class="contact_info_box">
          <div class="addr">
            5F,No.38,Sec.3,<br />Chongqing S.Rd.Zhongzheng Dist.,Taipei City
            100056<br />
            Taiwan(R.O.C.)
          </div>
          <div class="copyright">@2022 OMX All rights reserved</div>
        </div>
        <hr />
      </div>
    </div>
  </div>
</template>
<style scoped>
.contact_index_box {
  color: #fff;
  height: 100vh;
  background: #6d7270;
  padding: 150px 0;
  position: relative;
}
.plus {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.contact_index_box .contact_index {
  display: flex;
  flex-direction: column;
}
.contact_index_box .layout {
}
.contact_index_box .sub_title {
  margin-top: 50px;
}
.contact_index_box .title {
  font-size: 3em;
}
.contact_index_box .icon_box {
  display: flex;
  justify-content: flex-end;
  margin-bottom: 20px;
}
.contact_index_box .icon_box a {
  color: #fff;
}
.contact_index_box .icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 1px solid #fff;
  margin-left: 10px;
  position: relative;
  transition: 0.4s;
}
.contact_index_box .icon:hover {
  opacity: 0.5;
  border: 3px solid #fff;
}
.contact_index_box .icon .svg-inline--fa {
  font-size: 10px;
}
.contact_index_box .contact_bottom {
  position: absolute;
  width: 85%;
  bottom: 20px;
}
.contact_index_box .contact_info_box {
  font-size: 14px;
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
