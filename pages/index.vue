<template>
  <div class="container">
    <headbar :msg="number"  @numberChanged="number = $event"></headbar>
    <Content />
    <Slider />
    <AboutUs /> 
    <Footer />
  </div>
</template>

<script>
import headbar from '~/components/headbar.vue'
import Content from '~/components/Content.vue'
import Slider from '~/components/Slider.vue'
import AboutUs from '~/components/aboutUs.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    headbar,
    Content,
    Slider,
    AboutUs,
    Footer
  }
}
</script>

<style lang="sass" scoped>

</style>
