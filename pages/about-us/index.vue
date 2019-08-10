<template>
  <div class="container">
    <headbar />
    <Content />
    <AboutUs />
    <Footer />
  </div>
</template>

<script>
import headbar from '~/components/headbar.vue'
import Content from '~/components/Content.vue'
import AboutUs from '~/components/aboutUs.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    headbar,
    Content,
    AboutUs,
    Footer
  }
}
</script>

<style lang="sass">
@media screen and (max-width: 768px)
  .text
    margin-bottom: 2%
.button
  display: none
</style>
