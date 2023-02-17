<template>
  <div class="service_contact_box">
    <div class="inbox layout">
      <div class="plus">
        <i class="fa-solid fa-plus"></i>
      </div>
      <div class="sub_title">With new business inquiry</div>
    </div>
    <div class="footer_layout">
      <div class="inbox contact_bottom">
        <div class="time_icon">
          <div class="time">
            <p>TAIPEI | GMT +8 | 22:14 | Tuesday,23 | 2022</p>
          </div>
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
        </div>
        <hr />
        <div class="contact_info_box">
          <div class="addr">
            5F,No.38,Sec.3,<br />Chongqing S.Rd.Zhongzheng Dist.,Taipei City
            100056<br />
            Taiwan(R.O.C.)
          </div>
          <div class="phone_mail">
            <p>T +886-2-23924359</p>
            <p>F +886-2-23926816</p>
            <p>E info@xxtrralab.tw</p>
          </div>
          <div class="copyright">@2022 OMX All rights reserved</div>
        </div>
        <hr />
      </div>
    </div>
  </div>
</template>
<style scoped>
.service_contact_box {
  color: #6d7270;
  height: 100vh;
  background-color: #d6dfd9;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
}

.service_contact_box .plus {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.service_contact_box .title {
  font-size: 3em;
}
.service_contact_box .time_icon {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.service_contact_box .icon_box {
  display: flex;
  justify-content: flex-end;
  margin-bottom: 20px;
}
.service_contact_box .icon_box a {
  color: #fff;
}
.service_contact_box .icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 1px solid #fff;
  margin-left: 10px;
  position: relative;
  transition: 0.4s;
}
.service_contact_box .icon:hover {
  opacity: 0.5;
  border: 3px solid #fff;
}
.service_contact_box .icon .svg-inline--fa {
  font-size: 10px;
}
.service_contact_box .layout {
  position: relative;
  margin: 25vh 0 0;
}
.service_contact_box .footer_layout {
  background: #6d7270;
  position: relative;
  color: #fff;
  width: 100%;
  min-height: 250px;
  padding: 30px;
}

.service_contact_box .contact_info_box {
  font-size: 14px;
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.service_contact_box .contact_info_box .phone_mail {
  display: flex;
  justify-content: space-between;
}
.service_contact_box .svg-inline--fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 2.5em;
}
</style>
