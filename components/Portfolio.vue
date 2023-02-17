<template>
  <div id="portfolio" class="home_sec6">
    <section class="about_sec_box">
      <div class="service_sec">
        <div class="pic">
          <img class="cover-fit" src="/images/img_index_banner04.jpg" alt="" />
        </div>
        <div class="space">
          <div class="content_info">
            <div class="title">Ｏ</div>
            <div class="content">
              we combined our service to improve the best for our customer.The
              standard chunk of torem Ipsum used since the 1500s is reproduced
              below for those interested .Sections 1,10,32 and 1.10.33 from
              “deFinibus Bonoruum et Malorum”
            </div>
            <div class="btn">
              <a href="/portfolio_page" class="btn_link">
                <i class="fa-solid fa-arrow-right-long"></i> READ MORE
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="service_sec">
        <div class="pic pic2">
          <img class="cover-fit" src="/images/img_index_banner04.jpg" alt="" />
        </div>
        <div class="space space2">
          <div class="content_info">
            <div class="title">XXTRALAB</div>
            <div class="content">
              we combined our service to improve the best for our customer.The
              standard chunk of torem Ipsum used since the 1500s is reproduced
              below for those interested .Sections 1,10,32 and 1.10.33 from
              “deFinibus Bonoruum et Malorum”
            </div>
          </div>
          <div class="btn">
            <a href="/portfolio_page" class="btn_link">
              <i class="fa-solid fa-arrow-right-long"></i> READ MORE
            </a>
          </div>
        </div>
      </div>
      <div id="contact" class="contact_index_box">
        <div class="plus">
          <i class="fa-solid fa-plus"></i>
        </div>

        <div class="inbox layout">
          <div class="contact_index">
            <h1 class="title">Contact Us</h1>
            <div class="sub_title">With new business inquiry</div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<style scoped>
.about_sec_box {
  color: #6d7270;
}

.about_sec_box .service_sec {
  justify-content: center;
  display: flex;
  align-items: center;
  height: 50vh;
  background: #d6dfd9;
}
.about_sec_box .pic {
  width: 50vw;
  height: 100%;
}
.about_sec_box .space {
  width: 50vw;
  padding: 40px;
  /* display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100%; */
}

.about_sec_box .space .title {
  margin: 20px 0;
  font-size: 32px;
}

.about_sec_box .space .btn {
  background: #6d7270;
  color: #fff;
  padding: 10px;
  font-size: 14px;
  border-radius: 20px;
  margin-top: 28px;
  display: inline-block;
  cursor: pointer;
  border: 1px solid transparent;
  transition: all 0.3s ease-in-out;
}
.about_sec_box .space .btn:hover {
  background: transparent;
  color: #6d7270;
  border: 1px solid #6d7270;
}
.about_sec_box .space .btn .fa-arrow-right-long {
  margin-right: 10px;
}
.service_sec .pic2 {
  order: 2;
}
.about_sec_box .service_sec .space2 {
  order: 1;
}

.contact_index_box {
  color: #fff;
  height: 100vh;
  background: #6d7270;
  position: relative;
  display: flex;
  justify-content: center;
}
.contact_index_box .plus {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.contact_index_box .plus .svg-inline--fa {
  font-size: 50px;
}
.contact_index_box .layout {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.contact_index_box .sub_title {
  margin-top: 50px;
}
.contact_index_box .title {
  font-size: 3em;
}
</style>
