<template>
  <div class="home_item">
    <ul class="ulli">
      <li><a class="active" href="#exhibition">EXHIBITION</a></li>
      <li><a href="#interior">INTERIOR DESIGN</a></li>
      <li><a href="#interection">INTERECTION</a></li>
    </ul>
  </div>
</template>
<script>
export default {
  mounted() {
    window.jQuery('.home_item ul li').on('click', function () {
      window.jQuery(this).find('a').addClass('active')
      window.jQuery(this).siblings().find('a').removeClass('active')
    })
  },
}
</script>
<style scoped>
.home_item {
  text-align: left;
  z-index: 9;
}
.home_item a {
  font-size: 28px;
  color: #fff;
  opacity: 0.5;
}
.home_item a:hover,
.home_item a.active {
  opacity: 1;
}
.home_item a.active {
  cursor: default;
}
</style>
