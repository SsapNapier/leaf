<template>
  <div class="Contact-form">
    <div class="form">
      <div class="contact-logo">
        <!-- <div class="contact-img">
          <img src="456.svg" alt="">
        </div>
        <div class="contac-phone">
          <h3>Phone: (+2 392 3929 210 )</h3>
        </div>
        <div class="contact-email">
          <h3>Email: info@yourdomain.com</h3>
        </div> -->
        <!-- <iframe src=" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe> -->
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d32981.90024662283!2d-0.15323207465611371!3d51.50856144728529!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47d8a00baf21de75%3A0x52963a5addd52a99!2zzpvOv869zrTOr869zr8sIM6Xzr3Pic68zq3Ovc6_IM6SzrHPg86vzrvOtc65zr8!5e1!3m2!1sel!2s!4v1563095326313!5m2!1sel!2s" frameborder="0" style="border:0" allowfullscreen></iframe>
      </div>
      <div class="text-form">
        <div class="contact">
          <h2>CONTACT WITH US</h2>
        </div>
        <div class="name-form">
          <h5>Your name</h5>
          <input type="text" name="" value="">
        </div>
        <div class="mail-form">
          <h5>Your email</h5>
          <input type="text" name="" value="">
        </div>
        <div class="message-form">
          <h5>Your message</h5>
          <input type="text" name="" value="">
        </div>
        <div class="button">
          <button type="button" v-on:click="changeColor" name="button">Send message</button>
        </div>
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
.Contact-form
  position: relative
  top: 0px
  background: white
  color: black
  font-family: Rowland-Light
  width: 100%
  margin: 0 auto
.contact
  text-align: center
.contact h2
  font-size: 3rem
  font-weight: 300
.contact-logo iframe
  width: 100%
  height: 100%
  -webkit-filter: brightness(0.8)
.form
  display: flex
  width: 100%
  margin: 0 auto
@media screen and (max-width: 768px)
  .form
    flex-direction: column-reverse
.contact-logo
  width: 44%
.contact-logo h3
  font-size: 1.8rem
  font-weight: 300
@media screen and (max-width: 768px)
  .contact-logo
    width: 100%
    height: 250px
.text-form
  width: 36%
  display: flex
  flex-direction: column
  margin: 0 auto
@media screen and (max-width: 768px)
  .text-form
    width: 80%
    display: flex
    flex-direction: column
    margin: 0 auto
@media screen and (max-width: 1024px)
  .text-form
    margin-top: 2%
.text-form
  position: relative
  top: 0
  // padding-top: 0%
.text-form div input
  width: 100%
.name-form input
  height: 40px
.mail-form input
  height: 40px
.text-form div h5
  padding-bottom: 2%
  padding-top: 1%
  font-size: 1.4rem
  font-weight: 300
.message-form input
  padding-top: 10px
  padding-bottom: 140px
.button
  display: flex
  margin: 0 auto
  margin-top: 5%
  margin-bottom: 5%
  align-items: center
.button button
  background: #24a474
  border: 1px solid black
  color: white
  border-radius: 20px
  padding: 10px
  width: 140px
  font-size: 0.8rem
  font-weight: 300
</style>
