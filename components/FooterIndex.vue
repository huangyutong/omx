<template>
  <div class="home_footer_bottom">
    <div class="inbox_contact">
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
      <div class="info_box">
        <div class="addr">
          5F,No.38,Sec.3,<br />Chongqing S.Rd.Zhongzheng Dist.,Taipei City
          100056<br />
          Taiwan(R.O.C.)
        </div>
        <div class="tel_box">
          <div class="tel">T +886-2-23924359</div>
          <div class="fax">F +886-2-23926816</div>
          <div class="mail">E info@xxtrralab.tw</div>
        </div>
        <div class="copyright">@2022 OMX All rights reserved</div>
      </div>
      <hr />
    </div>
  </div>
</template>
<style>
.home_footer_bottom {
  background: #6d7270;
  color: #fff;
  padding: 20px 0;
}
.home_footer_bottom .icon_box {
  display: flex;
  justify-content: flex-end;
  margin-bottom: 20px;
}
.home_footer_bottom .icon_box a {
  color: #fff;
}
.home_footer_bottom .icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 1px solid #fff;
  margin-left: 10px;
  position: relative;
  transition: 0.4s;
}
.home_footer_bottom .icon:hover {
  opacity: 0.5;
  border: 3px solid #fff;
}
.home_footer_bottom .icon .svg-inline--fa {
  font-size: 10px;
}
.home_footer_bottom .contact_bottom {
  position: absolute;
  width: 85%;
  bottom: 20px;
}
.home_footer_bottom .info_box {
  font-size: 14px;
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
}
.home_footer_bottom .info_box .addr {
  line-height: 20px;
}
.home_footer_bottom .info_box .tel_box {
  display: flex;
  gap: 10px;
}

.home_footer_bottom .svg-inline--fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 2.5em;
}
@media screen and (max-width: 1080px) {
  .home_footer_bottom .info_box {
    flex-wrap: wrap;
    gap: 15px;
  }
}
@media screen and (max-width: 768px) {
  .home_footer_bottom .info_box .addr {
    width: 100%;
  }
}
@media screen and (max-width: 500px) {
  .home_footer_bottom .addr {
    text-align: center;
  }
  .home_footer_bottom .info_box,
  .home_footer_bottom .info_box .tel_box {
    flex-direction: column;
  }
}
</style>
