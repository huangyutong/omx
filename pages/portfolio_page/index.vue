<template>
  <div class="portfolio_page">
    <!-- <Navbar /> -->
    <PortfolioBanner />
    <div class="portfolio_list inbox">
      <div class="project">
        <a href="" class="project_link">
          <img src="/images/img_portfolio_list.jpg" alt="" class="cover-fit" />
        </a>
        <div class="project_info">
          <div class="project_title">O</div>
        </div>
      </div>
    </div>
    <!-- <FooterIndex /> -->
  </div>
</template>

<script>
export default {}
</script>
<style>
.portfolio_page {
  background: #d6dfd9;
}
.portfolio_page .portfolio_list .project {
  position: relative;
  overflow: hidden;
  margin-bottom: 40px;
}
.portfolio_page .portfolio_list .project .project_info {
  position: absolute;
  background-color: rgba(0, 0, 0, 0.5);
  color: #fff;
  padding: 30px;
  width: 100%;
  bottom: -100px;
  transition: all 0.4s ease-in-out;
  visibility: hidden;
}
.portfolio_page .portfolio_list .project .project_link {
  display: block;
}
.portfolio_page .portfolio_list .project:hover .project_info {
  visibility: visible;
  bottom: 0;
}
</style>
