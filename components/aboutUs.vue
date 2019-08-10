<template>
   <div class="container">
      <div class="text-block">
         <div class="headline">
             <h2>About us and what we are doing here</h2>
         </div>
         <hr>
         <div class="text">
                 <p>Pellentesque vestibulum dui quam, sed varius dui placerat ac. Integer elementum tortor purus, a bibendum turpis fringilla a. Cras consectetur id erat ac tristique. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nunc eu mollis ipsum. Aliquam viverra tortor quis bibendum sodales. Nullam in elit at arcu gravida consequat. Quisque id dapibus tortor, et congue urna. </p>
         </div>
         <div class="button">
           <a href="https://ssapnapier.github.io/about-us/">
             <button type="button" href="https://ssapnapier.github.io/about-us/" name="button">Read more</button>
           </a>
         </div>
      </div>
      <div class="photo-block">
        <img src="https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/lotKaktus.jpg" alt="">
      </div>
   </div>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
.container
  display: flex
  width: 90%
  justify-content: space-around
  margin: 0 auto
  font-family: Rowland-Light
  margin-top: 4%
  margin-bottom: 2%
@media screen and (max-width: 1024px)
  .container
    width: 95%
@media screen and (max-width: 768px)
  .container
    flex-direction: column
    text-align: center
    align-items: center
.text-block
  width: 40%
  display: flex
  flex-direction: column
@media screen and (max-width: 1024px)
  .text-block
    width: 45%
@media screen and (max-width: 768px)
  .text-block
   width: 90%
   align-items: center
.headline
  display: flex
  width: 75%
.headline h2
  font-size: 2.4rem
  font-weight: 100
  padding-bottom: 2%
@media screen and (max-width: 1024px)
  .headline h2
    font-size: 2rem
hr
  width: 195px
.text
  display: flex
  padding-top: 3%
.text p
  font-size: 1.2rem
@media screen and (max-width: 768px)
  .headline
    width: auto
    display: flex
    margin: 0 auto
  hr
    width: 80%
@media screen and (max-width: 1024px)
  .text p
    font-size: 1.1rem
.button
  margin-top: 3%
.button button
  background: none
  border: 1px solid black
  height: 30px
  width: 30%
  font-size: 1.1rem
  color: black
@media screen and (max-width: 1024px)
  .button button
    width: 40%
@media screen and (max-width: 768px)
  .button button
    width: 100%
    margin-bottom: 13%
.button button:hover
  background: #f2f2f2
.photo-block
  display: flex
  width: 40%
.photo-block img
  width: 100%
  height: 100%
@media screen and (max-width: 1024px)
  .photo-block
    display: flex
    width: 45%
  .photo-block img
    height: 100%
@media screen and (max-width: 768px)
  .photo-block
    width: 80%
</style>
