<template>
  <div class="home">
    <FirstBanner />
    <AboutusIndex />
    <ExhibitionIndex />
    <InteriorDesign />
    <Interection />
    <Portfolio />
    <ContactIndex />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  mounted() {
    // const btnScrollDown = document.querySelector('#circle .scroll')
    // function scrollDown() {
    //   const windowCoords = document.documentElement.clientHeight
    //   ;(function scroll() {
    //     if (window.pageYOffset < windowCoords) {
    //       window.scrollBy(0, 10)
    //       setTimeout(scroll, 0)
    //     }
    //     if (window.pageYOffset > windowCoords) {
    //       window.scrollTo(0, windowCoords)
    //     }
    //   })()
    // }
    // btnScrollDown.addEventListener('click', scrollDown)
  },
}
</script>
<style></style>
