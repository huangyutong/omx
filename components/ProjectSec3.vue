<template>
  <div class="gallery_box">
    <div class="inbox">
      <h1>GALLERY</h1>
      <ul class="ulli">
        <li>
          <div class="project_box">
            <div class="project_name">YOUNG ART AWARD MEMORIES</div>
            <div class="project_customer">NATIONAL THEATER</div>
            <div class="icon"></div>
          </div>
          <div class="content_box">
            <div class="wrapper">
              <div class="pic">
                <img
                  class="cover-fit"
                  src="/images/img_index_banner.jpg"
                  alt=""
                />
              </div>
              <div class="info">
                <div class="name">YOUNG ART AWARD MEMORIES</div>
                <div class="year">2017</div>
                <div class="customer">NATIONAL THEATER</div>
                <p>
                  we combined our service to improve the best for our customer.
                  The standard chunk of Lorem Ipsum used since the 1500s is
                  reproduced below for those interested. Sections 1.10.32 and
                  1.10.33 from “de Finibus Bonorum et Malorum” by Cicero are
                  also reproduced in their exact original from,accompanied by
                  English verions from the 1914 translation by H. Rackham.
                </p>
              </div>
            </div>
          </div>
        </li>
        <li>
          <div class="project_box">
            <div class="project_name">YOUNG ART AWARD MEMORIES</div>
            <div class="project_customer">NATIONAL THEATER</div>
            <div class="icon"></div>
          </div>
          <div class="content_box">
            <div class="wrapper">
              <div class="pic">
                <img
                  class="cover-fit"
                  src="/images/img_index_banner.jpg"
                  alt=""
                />
              </div>
              <div class="info">
                <div class="name">YOUNG ART AWARD MEMORIES</div>
                <div class="year">2017</div>
                <div class="customer">NATIONAL THEATER</div>
                <p>
                  we combined our service to improve the best for our customer.
                  The standard chunk of Lorem Ipsum used since the 1500s is
                  reproduced below for those interested. Sections 1.10.32 and
                  1.10.33 from “de Finibus Bonorum et Malorum” by Cicero are
                  also reproduced in their exact original from,accompanied by
                  English verions from the 1914 translation by H. Rackham.
                </p>
              </div>
            </div>
          </div>
        </li>
        <li>
          <div class="project_box">
            <div class="project_name">YOUNG ART AWARD MEMORIES</div>
            <div class="project_customer">NATIONAL THEATER</div>
            <div class="icon"></div>
          </div>
          <div class="content_box">
            <div class="wrapper">
              <div class="pic">
                <img
                  class="cover-fit"
                  src="/images/img_index_banner.jpg"
                  alt=""
                />
              </div>
              <div class="info">
                <div class="name">YOUNG ART AWARD MEMORIES</div>
                <div class="year">2017</div>
                <div class="customer">NATIONAL THEATER</div>
                <p>
                  we combined our service to improve the best for our customer.
                  The standard chunk of Lorem Ipsum used since the 1500s is
                  reproduced below for those interested. Sections 1.10.32 and
                  1.10.33 from “de Finibus Bonorum et Malorum” by Cicero are
                  also reproduced in their exact original from,accompanied by
                  English verions from the 1914 translation by H. Rackham.
                </p>
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    window.jQuery('.gallery_box ul > li').click(function () {
      window.jQuery(this).find('.content_box').slideToggle('fast')

      window.jQuery(this).find('.icon').toggleClass('close')
      // window.jQuery(this).toggleClass('active')
      // window.jQuery(this).find('.content_box').siblings().removeClass('on')
    })
  },
}
</script>
<style>
.gallery_box {
  background: #d6dfda;
  padding: 50px 0 150px;
}
.gallery_box ul li {
  border-bottom: 1px solid #111;
  padding: 20px 0;
  position: relative;
}
.gallery_box .project_box {
  display: flex;
  justify-content: space-between;
}
.gallery_box .project_box .icon {
  width: 30px;
  height: 30px;
  /* background: #000; */
  position: relative;
}
.gallery_box .project_box .icon:after {
  cursor: pointer;
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  background-image: url('/images/icon_project_plus.svg');
  background-size: contain;
  background-repeat: no-repeat;
}
.gallery_box .project_box .icon.close:after {
  cursor: pointer;
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  background-image: url('/images/icon_project_minus.svg');
  background-size: contain;
  background-repeat: no-repeat;
}
.gallery_box ul li .content_box {
  /* position: absolute;
  top: 80px; */
  display: none;
  margin: 50px 0;
}
.gallery_box ul li .content_box .wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
}
.gallery_box ul li .content_box .pic {
  display: inline-block;
}
.gallery_box .content_box .info {
  display: inline-block;

  padding: 0 20px;
}
</style>
