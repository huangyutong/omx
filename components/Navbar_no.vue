<template>
  <div class="navbar inbox">
    <div class="logo_title">OMX</div>
    <nav>
      <ul class="ulli">
        <li><a href="/about_page">ABOUT US</a></li>
        <li><a href="/service_page">SERVICE</a></li>
        <li><a href="/portfolio_page">PORTFOLIO</a></li>
        <li><a href="/contact_page">CONTACT</a></li>
        <li><a href="">EN</a></li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
.navbar {
  height: 60px;
  color: #f2f2f2;
  display: flex;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  justify-content: space-between;
  align-items: center;
  z-index: 100;
}
.navbar nav ul {
  display: flex;
}
.navbar nav ul li a {
  color: #f2f2f2;
  display: block;
  margin: 0px 10px;
}
</style>
