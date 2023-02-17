<template>
  <div class="service_contact_box">
    <div></div>
    <div class="inbox layout">
      <!-- <div class="plus">
        <i class="fa-solid fa-plus"></i>
      </div> -->
      <div class="sub_title">
        Contact Us <br />
        With <br />New business inquiry
      </div>
    </div>
    <div class="time_icon inbox">
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
.service_contact_box .time_icon {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.service_contact_box .time_icon .icon_box {
  display: flex;
  justify-content: flex-end;
  margin-bottom: 20px;
}
.service_contact_box .time_icon .icon_box a {
  color: #6d7270;
}
.service_contact_box .time_icon .icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 1px solid #6d7270;
  margin-left: 10px;
  position: relative;
  transition: 0.4s;
}
.service_contact_box .time_icon .icon:hover {
  opacity: 0.5;
  border: 3px solid #fff;
}
.service_contact_box .time_icon .icon .svg-inline--fa {
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
