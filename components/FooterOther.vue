<template>
  <div class="footer_layout">
    <div class="inbox contact_bottom">
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
</template>
<style>
.footer_layout {
  background: #575b5a;
  color: #fff;
  padding: 20px 0;
}
.footer_layout .title {
  font-size: 3em;
}

.footer_layout .layout {
  position: relative;
  margin: 25vh 0 0;
}
.footer_layout .footer_layout {
  background: #6d7270;
  position: relative;
  color: #fff;
  width: 100%;
  min-height: 250px;
  padding: 30px;
}

.footer_layout .contact_info_box {
  font-size: 14px;
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.footer_layout .contact_info_box .phone_mail {
  display: flex;
  justify-content: space-between;
}
.footer_layout .svg-inline--fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 2.5em;
}
</style>
