<template>
  <div>
    <section class="service_sec_box">
      <div class="inbox">
        <div class="p_a">
          <div class="service_item">
            <ul class="ulli">
              <li><a href="">EXHIBITION</a></li>
              <li><a class="active" href="">INTERIOR DESIGN</a></li>
              <li><a href="">INTERECTION</a></li>
            </ul>
          </div>
          <div class="service_content">
            <p>
              we combined our service to improve the best for our customer.The
              standard chunk of torem Ipsum used since the 1500s is reproduced
              below for those interested .Sections 1,10,32 and 1.10.33 from
              “deFinibus Bonoruum et Malorum”
            </p>
            <div class="read_more">
              <i class="fa-solid fa-plus"></i>
              <a href="">READ MORE</a>
            </div>
          </div>
        </div>
      </div>
      <div class="service_sec">
        <div class="pic">
          <img class="cover-fit" src="/images/img_index_banner04.jpg" alt="" />
        </div>
        <div class="space"></div>
      </div>
      <div class="service_sec">
        <div class="pic pic2">
          <img class="cover-fit" src="/images/img_index_banner04.jpg" alt="" />
        </div>
        <div class="space space2"></div>
      </div>
    </section>
  </div>
</template>
<style scoped>
.service_sec_box {
  color: #fff;
}
.service_sec_box .inbox {
  position: relative;
}
.service_sec_box .p_a {
  /* padding: 100px 0px; */
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  position: absolute;
  top: 0;
  left: 0;
  height: 100vh;
}
.service_sec_box .service_item {
  /* position: absolute; */
  top: 46px;
  left: 0;
  text-align: left;
  z-index: 5;
}

.service_sec_box .service_item a {
  font-size: 36px;
  color: #fff;
  opacity: 0.5;
}
.service_sec_box .service_item a:hover,
.service_sec_box .service_item a.active {
  opacity: 1;
}
.service_sec_box .service_item a.active {
  cursor: default;
}
.service_sec_box li {
  line-height: 40px;
}
.service_sec_box .service_content {
  text-align: left;
  margin: 150px 0px 40px;
  max-width: 65%;
}
.service_sec_box .read_more {
  padding: 10px 20px;
  border-radius: 30px;
  border: 1px solid #fff;
  display: flex;
  align-items: center;
  max-width: 200px;
  margin-top: 40px;
}
.service_sec_box .read_more a {
  display: block;
  color: #fff;
  white-space: nowrap;
}
.service_sec_box .read_more .svg-inline--fa {
  border: 1px solid #fff;
  border-radius: 50%;
  position: static;
  width: 20px;
  height: 20px;
  padding: 5px;
  margin-right: 20px;
}
.service_sec_box .service_sec {
  justify-content: center;
  display: flex;
  height: 50vh;
}
.service_sec_box .pic {
  width: 50vw;
}
.service_sec_box .space {
  background: #575b5a;
  width: 50vw;
}
.service_sec .pic2 {
  order: 2;
}
.service_sec_box .service_sec .space2 {
  order: 1;
  flex-direction: column-reverse;
}
</style>
