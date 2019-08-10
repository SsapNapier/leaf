щ<template>
  <div class="Content">
    <div class="main-photo">
      <img src="https://raw.githubusercontent.com/SsapNapier/ssapnapier.github.io/master/kaktus.jpg" alt="">
      <div class="block">
          <h4>the shope</h4>
          <h4>Sale 	| online</h4>
      </div>
    </div>
    <div class="info-block">
      <div class="title">
        <h2>Design solutions for<br> interiors </h2>
      </div>
      <hr>
      <div class="product-description">
        <p>Lorem ipsum dolor sit amet,<br>
           consectetur adipiscing elit.<br>
           Sed augue dolor, condimentum<br>
           nec convallis ut, pellentesque<br>
           non ipsum. Pellentesque et dapibus<br>
           nunc. Proin sed pulvinar leo, porta<br>
           ullamcorper mi. Donec accumsan magna id</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
.Content
  display: flex
  font-family: Rowland-Light
.main-photo
  z-index: 1
  width: 44%
.main-photo img
  width: 100%
.info-block
  margin: 0 auto
  padding-top: 13%
.title
  margin-bottom: 2%
.title h2
  font-size: 3rem
  font-weight: 400
@media screen and (max-width: 1024px)
  .info-block
    margin-left: 12%
    padding-top: 16%
  .title h2
    font-size: 2rem
@media screen and (max-width: 768px)
   .info-block
     width: 43%
     margin-left: 10%
   .main-photo
     width: 45%
   .main-photo img
     width: 100%
     float: right
   .Content
     width: 100%
   .title h2
     font-size: 1.7rem
@media screen and (max-width: 480px)
  .Content
    flex-direction: column
    position: relative
    top: 70px
  .main-photo
    width: 100%
  .info-block
    display: flex
    flex-direction: column
    width: auto
    text-align: center
    margin: 0 auto
    margin-top: -10%
    margin-bottom: 22%
    padding-top: 0%
    z-index: 2
    align-items: center
  .title h2
    flex-shrink: 0
    font-size: 2.2rem
hr
  width: 52%
.product-description
  margin-top: 4%
.product-description p
  font-weight: 400
  font-size: 1.5rem
@media screen and (max-width: 1024px)
  hr
    width: 40%
  .product-description p
    font-weight: 400
    font-size: 1.2rem
@media screen and (max-width: 768px)
  .product-description p
    font-weight: 400
    font-size: 1.128rem
  hr
    width: 32%
@media screen and (max-width: 480px)
  .product-description p
    font-weight: 400
    font-size: 1.1rem
.block
  position: relative
  display: flex
  width: 50%
  height: 79px
  font-weight: 500
  justify-content: space-around
  align-items: center
  margin:
     top: -85px
     left: 64.4%
  padding-top: 1%
  color: white
  background: #177d56
  z-index: 3000
.block h4
  font-size: 1.25rem
  font-family: Rowland
  font-weight: 100
@media screen and (max-width: 768px)
  .block
    position: relative
    width: 100%
    margin:
       top: 85px
       left: 0%
@media screen and (max-width: 480px)
  .block
    position: relative
    top: -80px
    width: 50%
    z-index: 3000
    margin:
       top: -0px
       left: 50%
  .block h4
    font-size: 1.1rem
</style>
