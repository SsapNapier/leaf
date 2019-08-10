<template>
  <div class="container">
    <headbar :evt="number" @number="number = $event"></headbar>
    <Content />
    <Shop :PlantImg="PlantImg"
          :plants="plants" :i="i"  @valueModal="i = $event" :PlantPrice="PlantPrice"
          :msg="displayActive" @numberChanged="displayActive = $event" ></Shop>
    <modalWindow :PlantImg="PlantImg"
                 :plants="plants" :i="i" @valueModal="i = $event"
                 :PlantPrice="PlantPrice" :evt="number" @number="number = $event" :msg="displayActive"  @numberChanged="displayActive = $event"></modalWindow>
    <Footer />
  </div>
</template>
:msg="displayActive"  @numberChanged="displayActive = $event"
<script>
import headbar from '~/components/headbar.vue'
import Content from '~/components/Content.vue'
import Shop from '~/components/Shop.vue'
import modalWindow from "~/components/modalWindow.vue"
import Footer from '~/components/Footer.vue'

export default {
  data(){
    return{
       evt: 0,
       i: 1,
       number: 0,
       displayActive: 'none',
       plants: ["Hyacinth", "Mattiola", "Freesia", "Eustoma", "Hyacinth", "Mattiola", "Freesia", "Eustoma", "Hyacinth", "Mattiola", "Freesia", "Eustoma", "Hyacinth", "Mattiola", "Freesia", "Eustoma"],
       PlantPrice: ["$35", "$30", "$25", "$40", "$35", "$30", "$25", "$40", "$35", "$30", "$25", "$40", "$35", "$30", "$25", "$40"],
       PlantImg: ['https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/1.jpg', "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/3.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/12.jpeg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/10.jpg",
                  'https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/2.jpg', "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/7.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/9.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/6.jpg",
                  'https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/4.jpg', "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/5.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/11.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/8.jpg",
                  'https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/10.jpg', "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/12.jpeg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/6.jpg", "https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/products/7.jpg",]
    }
  },
  methods:{
  },
  components: {
    headbar,
    Content,
    Shop,
    modalWindow,
    Footer
  }
}
</script>

<style lang="sass" scoped>

</style>
