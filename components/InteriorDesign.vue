<template>
  <div>
    <section id="interior" class="interior_item_box">
      <div class="inbox">
        <!-- <div class="home_item">
          <ul class="ulli">
            <li><a href="#exhibition">EXHIBITION</a></li>
            <li><a class="active" href="#interior">INTERIOR DESIGN</a></li>
            <li><a href="#interection">INTERECTION</a></li>
          </ul>
        </div> -->
        <!-- <div class="masonry">
          <div class="item">
            <img
              class="cover-fit"
              src="https://picsum.photos/360/460?radom=1"
              alt=""
            />
          </div>
          <div class="item">
            <img
              class="cover-fit"
              src="https://picsum.photos/360/520?radom=2"
              alt=""
            />
          </div>
          <div class="item">
            <img
              class="cover-fit"
              src="https://picsum.photos/360/420?radom=3"
              alt=""
            />
          </div>
          <div class="item">
            <img
              class="cover-fit"
              src="https://picsum.photos/360/500?radom=4"
              alt=""
            />
          </div>
          <div class="item">
            <img
              class="cover-fit"
              src="https://picsum.photos/360/420?radom=5"
              alt=""
            />
          </div>
        </div> -->
        <ul class="interior-card">
          <li>
            <a href="/">
              <img class="cover-fit" src="/images/img-home-interior.jpg" />
              <div class="project-name">ALVA NOTO</div>
            </a>
          </li>
          <li>
            <a href="/">
              <img class="cover-fit" src="/images/img-home-interior-01.jpg" />
              <div class="project-name">ALVA NOTO</div>
            </a>
          </li>
          <li>
            <a href="/">
              <img class="cover-fit" src="/images/img-home-interior-02.jpg" />
              <div class="project-name">ALVA NOTO</div>
            </a>
          </li>
        </ul>
      </div>
      <!-- <div class="btn_circle">
        <a href="#" class="scroll">
          <i class="fa-solid fa-arrow-down"></i>
        </a>
      </div> -->
    </section>
  </div>
</template>
<script>
export default {
  mounted() {},
}
</script>
<style>
/* .masonry {
  column-count: 3;
  column-gap: 0;
} */
.interior_item_box {
  height: 100vh;
  background-color: hsl(140, 12%, 86%);
  position: relative;
}
.interior_item_box .inbox {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.interior_item_box .swiper-slide {
  height: inherit;
}
.interior-card {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.875rem;
}

.interior-card li {
  height: 100%;
  overflow: hidden;
}
.interior-card li a {
  display: block;
  position: relative;
  cursor: pointer;
}
.interior-card .project-name {
  padding: 30px 20px;
  position: absolute;
  background: rgba(0, 0, 0, 0.2);
  width: 100%;
  bottom: -200px;
  transition: all 0.4s ease-in-out;
  color: #fff;
}
.interior-card li a:hover .project-name {
  bottom: 0px;
}
@media only screen and (max-width: 992px) {
  .interior-card {
    grid-template-columns: repeat(1, minmax(0, 1fr));
  }
  .interior-card li {
    height: 25vh;
  }
}
/* .item {
  padding: 5px;
  position: relative;
  counter-increment: count;
}

.item img {
  display: block;
  width: 100%;
}
.item:nth-child(1) {
  height: 100vh;
}
.item:nth-child(2) {
  height: 40vh;
}
.item:nth-child(3) {
  height: 60vh;
}
.item:nth-child(4) {
  height: 70vh;
}
.item:nth-child(5) {
  height: 30vh;
} */
</style>
