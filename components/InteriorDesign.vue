<template>
  <div>
    <section class="index_item_box">
      <div class="inbox">
        <div class="home_item">
          <ul class="ulli">
            <li><a href="">EXHIBITION</a></li>
            <li><a class="active" href="">INTERIOR DESIGN</a></li>
            <li><a href="">INTERECTION</a></li>
          </ul>
        </div>
        <div class="fall inbox">
          <div class="layout_grid">
            <ul class="ulli">
              <li class="">
                <img
                  class="cover-fit"
                  src="/images/img_index_banneer02.jpg"
                  alt=""
                />
              </li>
              <li class="">
                <img
                  class="cover-fit"
                  src="/images/img_index_banneer02.jpg"
                  alt=""
                />
              </li>
              <li class="">
                <img
                  class="cover-fit"
                  src="/images/img_index_banneer02.jpg"
                  alt=""
                />
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="btn_circle">
        <i class="fa-solid fa-arrow-down"></i>
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
.index_item_box {
  height: 100vh;
  background-color: #d6dfd9;
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  color: #f2f2f2;
  display: flex;
  align-items: center;
  /* justify-content: space-around; */
  flex-direction: column;
  position: relative;
}
.index_item_box .inbox {
  position: relative;
}
.index_item_box:after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background: rgba(0, 0, 0, 0.2);
}
.index_item_box .home_item {
  position: absolute;
  top: 46px;
  left: 0;
  text-align: left;
  z-index: 5;
}
.index_item_box .home_item a {
  font-size: 28px;
  color: #fff;
  opacity: 0.5;
}
.index_item_box .home_item a:hover,
.index_item_box .home_item a.active {
  opacity: 1;
}
.index_item_box .home_item a.active {
  cursor: default;
}
.index_item_box .fall ul {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 40px 0;
}
.index_item_box .fall ul li {
  opacity: 0.7;
}
.index_item_box .fall ul li:hover {
  opacity: 1;
}
</style>
