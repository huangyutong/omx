<template>
  <div class="navbar inbox">
    <div class="logo_title"><a href="/">OMX</a></div>
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
<script>
export default {
  mounted() {
    const navbar = document.querySelector('.navbar')

    /**
     *
     * @param {event} e MouseWheel往下(opacity = "0")往上(opacity = "1")
     */

    function MouseWheel(e) {
      e = e || window.event
      e.wheelDelta <= 0 || e.detail > 0
        ? (navbar.style.opacity = '0')
        : (navbar.style.opacity = '1')
    }

    // hook event listener on window object
    if ('onmousewheel' in window) {
      window.onmousewheel = MouseWheel
    } else if ('onmousewheel' in document) {
      document.onmousewheel = MouseWheel
    } else if ('addEventListener' in window) {
      window.addEventListener('mousewheel', MouseWheel, false)
      window.addEventListener('DOMMouseScroll', MouseWheel, false)
    }
  },
}
</script>
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
.navbar a {
  color: #f2f2f2;
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
