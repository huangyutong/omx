<template>
  <div>
    <section class="service_box">
      <div class="inbox t_l">
        <div class="service_item">
          <ul class="ulli">
            <li><a href="">EXHIBITION</a></li>
            <li><a href="">INTERIOR DESIGN</a></li>
            <li><a class="active" href="">INTERECTION</a></li>
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
    </section>
  </div>
</template>
<script>
export default {
  mounted() {},
}
</script>
<style scoped>
.service_box {
  height: 100vh;
  background-image: url('/images/img_index_banner02.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  color: #f2f2f2;
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-direction: column;
  position: relative;
}
.service_box .inbox {
  position: relative;
}
.service_box :after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.2);
}
.service_box .service_item {
  /* position: absolute; */
  top: 46px;
  left: 0;
  text-align: left;
  z-index: 5;
}

.service_box .service_item a {
  font-size: 36px;
  color: #fff;
  opacity: 0.5;
}
.service_box .service_item a:hover,
.service_box .service_item a.active {
  opacity: 1;
}
.service_box .service_item a.active {
  cursor: default;
}
.service_box li {
  line-height: 40px;
}
.service_box .service_content {
  text-align: left;
  margin: 150px 0px 40px;
  max-width: 65%;
}
.service_box .read_more {
  padding: 10px 20px;
  border-radius: 30px;
  border: 1px solid #fff;
  display: flex;
  align-items: center;
  max-width: 200px;
  margin-top: 40px;
  white-space: nowrap;
}
.service_box .read_more a {
  display: block;
  color: #fff;
}
.service_box .read_more .svg-inline--fa {
  border: 1px solid #fff;
  border-radius: 50%;
  position: static;
  width: 20px;
  height: 20px;
  padding: 5px;
  margin-right: 20px;
}
</style>
