<template>
  <hooper :infiniteScroll="true">
    <slide>
      <div class="slide">
        <div class="slide-image">
          <img src="e-9VMIVs81o.jpg" alt="">
        </div>
        <div class="slide-logo">
          <h4>Meyer Tree</h4>
        </div>
        <div class="slide-price">
          <h4>20$</h4>
        </div>
        <div class="basket">
          <img src="shopping-cart.svg" alt="">
          <h5>add to bag</h5>
        </div>
      </div>
      <div class="slide">
        <div class="slide-image">
          <img src="VCpaeuFfpLw.jpg" alt="">
        </div>
        <div class="slide-logo">
          <h4>Korean Tree</h4>
        </div>
        <div class="slide-price">
          <h4>30$</h4>
        </div>
        <div class="basket">
          <img src="shopping-cart.svg" alt="">
          <h5>add to bag</h5>
        </div>
      </div>
    </slide>
    <slide>
      slide 2
    </slide>
    <slide>
      slide 3
    </slide>
    <slide>
      slide 4
    </slide>
    <slide>
      slide 5
    </slide>
    <slide>
      slide 6
    </slide>
  </hooper>
</template>

<script>
import { Hooper, Slide } from 'hooper';

export default {
  name: 'App',
  components: {
    Hooper,
    Slide
  }
}
</script>


<style lang="sass">
  .slide
    width: 14%
    margin: 2%
    border: 1.5px solid #03170b
    border-radius: 5px
    background: #c3ecdf
    overflow: hidden
    display: inline-flex
    justify-content: space-between
    flex-direction: column
  .slide-image
    height: 260px
    margin-bottom: 12%
  .slide-image img
    width: 100%
    box-shadow: 7px 5px 6px rgba(0,0,0,0.2)
  .slide-logo
    width: 80%
    margin: 0 auto
    margin-bottom: 6%
  .slide-logo h4
    font-size: 2rem
    font-weight: 400
  .slide-price
    width: 80%
    margin: 0 auto
    margin-bottom: 6%
  .slide-price h4
    font-size: 1.4rem
  .basket
    display: flex
    width: 80%
    margin: 0 auto
    background: #2f253e
    margin-bottom: 2%
    padding: 1%
    align-items: center
  .basket img
    width: 25px
  .basket h5
    color: white
    font-size: 1.2rem
    margin-left: 3%
    margin-top: 2%
</style>
