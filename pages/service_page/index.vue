<template>
  <div>
    <Navbar />
    <ServiceSec1 />
    <ServiceSec2 />
    <ServiceSec3 />
    <ServiceContact2 />
    <FooterOther />
  </div>
</template>

<script>
import FooterOther from '../../components/FooterOther.vue'
export default {
  name: 'IndexPage',
  components: { FooterOther },
}
</script>
