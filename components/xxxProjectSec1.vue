<template>
  <div>
    <section class="project_box">
      <div class="inbox t_l">
        <div class="project_item">
          <ul class="ulli">
            <li><a class="active" href="">EXHIBITION</a></li>
            <li><a href="">INTERIOR DESIGN</a></li>
            <li><a href="">INTERECTION</a></li>
          </ul>
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
.project_box {
  height: 100vh;
  background-image: url('/images/img_index_banner02.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  color: #f2f2f2;
  /* display: flex;
  align-items: center;
  justify-content: space-around;
  flex-direction: column; */
  position: relative;
}
.project_box .inbox {
  position: relative;
}

.project_box .project_item {
  position: absolute;
  top: 150px;
  left: 0;
  text-align: left;
  z-index: 5;
}

.project_box .project_item a {
  font-size: 36px;
  color: #fff;
  opacity: 0.5;
  position: relative;
}
.project_box .project_item a.active::after {
  content: '';
  width: 30px;
  height: 30px;
  color: #fff;
  background-image: url('/images/icon_project_down.svg');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  position: absolute;
  top: 50%;
  right: -30px;
  transform: translateY(-50%);
}
.project_box .project_item a:hover,
.project_box .project_item a.active {
  cursor: default;
  opacity: 1;
}
.project_box li {
  line-height: 40px;
}
.project_box .project_content {
  text-align: left;
  margin: 150px 0px 40px;
  max-width: 65%;
}
.project_box .read_more {
  padding: 10px 20px;
  border-radius: 30px;
  border: 1px solid #fff;
  display: flex;
  align-items: center;
  max-width: 200px;
  margin-top: 40px;
  white-space: nowrap;
}
.project_box .read_more a {
  display: block;
  color: #fff;
}
.project_box .read_more .svg-inline--fa {
  border: 1px solid #fff;
  border-radius: 50%;
  position: static;
  width: 20px;
  height: 20px;
  padding: 5px;
  margin-right: 20px;
}
</style>
