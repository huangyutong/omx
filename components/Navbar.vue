<template>
  <div class="navbar inbox">
    <div class="logo_title"><a href="/">OMX</a></div>
    <nav>
      <ul class="ulli">
        <li><a href="/#sec2">ABOUT US</a></li>
        <li><a href="/#exhibition">SERVICE</a></li>
        <li><a href="/#portfolio">PORTFOLIO</a></li>
        <li><a href="/#contact">CONTACT</a></li>
        <li><a href="">EN</a></li>
      </ul>
    </nav>
    <div class="menu-burger">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    window.jQuery('.menu-burger').click(function () {
      window.jQuery(this).parents('.navbar').toggleClass('menu-open')
      window.jQuery(this).parents('body').toggleClass('menu-open')
    })

    const navbar = document.querySelector('.navbar')

    // /**
    //  *
    //  * @param {event} e MouseWheel往下(opacity = "0")往上(opacity = "1")
    //  */

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
  border-bottom: 1px solid #f2f2f2;
  display: flex;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  justify-content: space-between;
  align-items: center;
  z-index: 1000;
}
.navbar nav {
  transition: right 0.4s ease-in-out;
}
.navbar nav ul {
  display: flex;
}
.navbar a {
  color: #f2f2f2;
}
.navbar nav ul li a {
  color: #f2f2f2;
  display: block;
  margin: 0px 10px;
}
.navbar a:hover {
  opacity: 0.6;
}
/* hamburger */
.navbar .menu-burger {
  display: none;
  left: 0;
  width: 24px;
  height: 20px;
  transform: rotate(0deg);
  transition: 0.5s ease-in-out;
  cursor: pointer;
  z-index: 9;
}

.navbar .menu-burger span {
  position: absolute;
  display: block;
  height: 3px;
  width: 100%;
  background: #fff;
  border-radius: 5px;
  opacity: 1;
  left: 0;
  transform: rotate(0deg);
  transform-origin: left center;
  transition: 0.25s ease-in-out;
}
.navbar .menu-burger span:nth-child(1) {
  top: 0px;
}
.navbar .menu-burger span:nth-child(2) {
  top: 8px;
}
.navbar .menu-burger span:nth-child(3) {
  top: 16px;
}
@media screen and (max-width: 768px) {
  .navbar nav {
    width: 100%;
    position: fixed;
    top: 0;
    bottom: 0;
    right: -100%;
    background: #000;
    display: block;
    z-index: 3;
  }
  .navbar nav ul {
    margin-top: 80px;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .navbar .menu-burger {
    display: block;
  }
  .navbar.menu-open .menu-burger span:nth-child(1) {
    transform: rotate(45deg);
    background-color: #fff;
  }

  .navbar.menu-open .menu-burger span:nth-child(2) {
    width: 0%;
    opacity: 0;
  }

  .navbar.menu-open .menu-burger span:nth-child(3) {
    transform: rotate(-45deg);
    top: 17px;
    background-color: #fff;
  }

  .navbar.menu-open nav {
    right: 0;
  }

  .navbar.menu-open .mb_menu_item {
    display: block;
  }
}
</style>
