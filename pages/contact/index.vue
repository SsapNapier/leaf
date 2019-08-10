<template>
  <div class="container">
    <headbar />
    <Content />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import headbar from '~/components/headbar.vue'
import Content from '~/components/Content.vue'
import Slider from '~/components/Slider.vue'
import Contact from '~/components/Contact.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    headbar,
    Content,
    Slider,
    Contact,
    Footer
  }
}
</script>

<style lang="sass" scoped>

</style>
