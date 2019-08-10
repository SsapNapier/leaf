<template>
  <div class="modal"
   v-bind:style="{ display: msg }">
      <div class="modal-content">
         <div class="img-content">
            <div class="price">
               <h4>{{ this.plants[this.i] + " " + this.PlantPrice[this.i] }}</h4>
            </div>
            <div class="plantImg">
               <img :src="this.PlantImg[this.i]" alt="">
            </div>
          </div>
            <div class="input-content">
              <div class="close">
                 <button type="button" v-on:click="number"  name="button">&times;</button>
              </div>
               <div class="Welcome">
                   <h3>WELCOME!</h3>
                   <h4>New items in the basket</h4>
               </div>
               <div class="input">
                   <input type="text"  name="" placeholder="Your email adress..." ><button type="button" name="button">ok</button>
               </div>
               <div class="amount">
                   <h3>Amount:</h3>
                   <button type="button" v-on:click="reduceNumber" name="button">	&#60; </button>
                   <span>&#160;{{ num }}</span>
                   <button type="button" @click="increaseNumber" name="button">&#62;</button>
               </div>
               <div class="cart">
                 <button type="button" name="button">To shopping</button>
                 <button type="button" @click="sendingNumber" name="button">Add to cart</button>
               </div>
            </div>
         </div>
      </div>
</template>

<script>
export default {
  props: ["msg", "evt", "plants", "PlantPrice", "i", "PlantImg"],
  data() {
    return {
      num: 0,
      msg: "",
      evt: ""
    }
  },
  methods:{
    number(event) {
      this.displayActive = "none"
      console.log(this.display);
      this.$emit("numberChanged", this.displayActive);
  },
  increaseNumber(){
    this.num = this.num + 1;
  },
  reduceNumber: function(){
    if(this.num <= 0){
       this.num = this.num;
    }else{
       this.num = this.num-1;
    }
  },
  sendingNumber(){
    if (localStorage.clickcount) {
      localStorage.clickcount = Number(localStorage.clickcount)+1;
    } else {
      localStorage.clickcount = 1;
    }
    localStorage.clickcount = this.num;
    this.number = localStorage.clickcount;
    this.$emit("number", this.number);
  },
  numberCount(event) {
    this.noumero = event.target.value;
  }
 }
}
</script>

<style lang="sass" scoped>
.modal
  position: fixed
  z-index: 3
  left: 0
  top: 0
  width: 100%
  height: 100%
  overflow: auto
  background-color: rgba(0,0,0,0.8)
.modal-content
  display: flex
  background-color: #fefefe
  margin: 15% auto
  margin-top: 10%
  margin-bottom: 8%
  border: 1px solid #888
  width: 600px
  height: 400px
@media screen and (max-width: 1024px)
  .modal-content
    width: 500px
    height: 300px
@media screen and (max-width: 768px)
  .modal-content
    margin-top: 16%
    width: 400px
    height: 350px
@media screen and (max-width: 480px)
  .modal-content
    width: 320px
.img-content
  width: 50%
  background: #d9d8d6
.price
  padding-top: 10%
  display: flex
  margin: 0 auto
  width: 70%
.price h4
  font-size: 2.1rem
  font-weight: 400
@media screen and (max-width: 1024px)
  .price
    padding-top: 10%
    display: flex
    margin: 0 auto
    width: 68%
  .price h4
    font-size: 1.8rem
    font-weight: 400
@media screen and (max-width: 768px)
  .price
    width: 80%
  .price h4
    font-size: 1.4rem
@media screen and (max-width: 480px)
  .price
    width: 80%
  .price h4
    font-size: 1.3rem
.plantImg
  display: flex
  justify-content: flex-end
  margin-top: 8%
.plantImg img
  height: 214px
  width: 60%
@media screen and (max-width: 1024px)
  .plantImg
    display: flex
    justify-content: flex-end
    margin-top: 4%
  .plantImg img
    height: 150px
    width: 50%
@media screen and (max-width: 768px)
  .plantImg img
    height: 200px
    width: 80%
@media screen and (max-width: 480px)
  .plantImg img
    width: 90%
.shopping
  margin-top: 6%
  display: flex
  justify-content: flex-end
.shopping button
  border: 1px solid black
  background: none
  width: 35%
  height: 30px
  font-size: 0.9rem
@media screen and (max-width: 1024px)
  .shopping button
    width: 50%
@media screen and (max-width: 768px)
  .shopping button
    width: 70%
.input-content
  width: 50%
  background: #e6e4e2
.Welcome
  padding-top: 36%
  display: flex
  flex-direction: column
  justify-content: center
  text-align: center
  color: #565656
  font-weight: 400
.Welcome h3
  font-size: 1.6rem
  padding-bottom: 3%
.Welcome h4
  font-size: 1.1rem
@media screen and (max-width: 1024px)
  .Welcome
    padding-top: 28%
  .Welcome h3
    font-size: 1.4rem
  .Welcome h4
    font-size: 0.9rem
@media screen and (max-width: 480px)
  .Welcome
    width: 100%
    text-align: center
    padding-top: 4%
.input
  display: flex
  justify-content: center
  padding-top: 4%
.input input
  height: 30px
  background: none
  border: 1px solid black
@media screen and (max-width: 768px)
  .input input
    width: 80%
.input button
  background: none
  border: 1px solid black
  border-left: 1px solid gray
@media screen and (max-width: 480px)
  .input
    flex-direction: column
    justify-content: center
    align-items: center
  .input input
    width: 100%
  .input button
    margin-top: 2%
    width: 30%
.amount
  padding-top: 12%
  display: flex
  margin: 0 auto
  width: 60%
@media screen and (max-width: 768px)
  .amount
    width: 74%
    padding-top: 20%
.amount button
  font-size: 1rem
  margin-top: -2%
  margin-left: 2%
  width: 10%
  padding: 1%
  background: #c5ccca
  border: none
.cart
  display: flex
  margin-left: -126px
  width: 120%
  padding-top: 19.6%
@media screen and (max-width: 1024px)
  .cart
    margin-left: - 125px
@media screen and (max-width: 768px)
  .cart
    margin-left: - 120px
@media screen and (max-width: 480px)
  .cart
    margin-left: -96px
.cart button
  background: none
  border: 1px solid black
  border-left: 1px solid gray
  width: 35%
  height: 30px
  font-size: 0.9rem
@media screen and (max-width: 1024px)
  .cart
    margin-top: -10.7%
  .cart button
      width: 50%
@media screen and (max-width: 768px)
  .cart
    margin-top: 21.4%
  .cart button
      width: 70%
@media screen and (max-width: 480px)
  .cart
    padding-top: 15.4%
.close
  color: #aaa
  float: right
  font-size: 28px
  font-weight: bold
.close button
  font-size: 2rem
  background: none
  border: none
</style>
