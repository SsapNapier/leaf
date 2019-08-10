<template>
   <div class="shop-container">
     <div class="inline-products">
       <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[0]" alt="">
           </div>
           <div class="product-name">
              <h4 >{{ this.plants[0] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[0] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" name="0" :value="msg" @click="numberChanged">Add to cart</button>
           </div>
         </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[1]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[1] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[1] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" name="1" :value="msg" @click="numberChanged">Add to cart</button>
           </div>
         </div>
        </div>
        <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[2]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[2] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[2] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="2">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[3]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[3] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[3] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="3">Add to cart</button>
           </div>
        </div>
        </div>
     </div>
     <div class="inline-products">
        <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[4]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[4] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[4] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="4">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[5]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[5] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[5] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="5">Add to cart</button>
           </div>
         </div>
        </div>
        <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[6]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[6] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[6] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="6">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[7]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[7] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[7] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="7">Add to cart</button>
           </div>
        </div>
      </div>
     </div>
     <div class="inline-products">
        <div class="double">
         <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[8]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[8] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[8] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="8">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[9]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[9] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[9] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="9">Add to cart</button>
           </div>
         </div>
        </div>
        <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[10]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[10] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[10] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="10">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[11]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[11] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[11] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="11">Add to cart</button>
           </div>
        </div>
      </div>
     </div>
     <div class="inline-products">
        <div class="double">
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[12]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[12] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[12] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="12">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[13]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[13] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[13] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="13">Add to cart</button>
           </div>
         </div>
        </div>
        <div class="double">
        <div class="product">
           <div
           class="product-img">
             <div class="product-buy">
             </div>
              <img :src="this.PlantImg[14]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[14] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[14] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="14">Add to cart</button>
           </div>
        </div>
        <div class="product">
           <div class="product-img">
              <img :src="this.PlantImg[15]" alt="">
           </div>
           <div class="product-name">
              <h4>{{ this.plants[15] }}</h4>
           </div>
           <div class="product-price">
              <h5>{{ this.PlantPrice[15] }}</h5>
           </div>
           <div class="product-button">
              <button type="button" :value="msg" @click="numberChanged" name="15">Add to cart</button>
           </div>
        </div>
      </div>
     </div>
   </div>
</template>

<script>
export default {
  props: ['msg', "evt", "plants", "PlantPrice", "i", "PlantImg"],
  data() {
    return{

         msg: 0,
         message: '',
         displayActive: "none",
         phones: ["samsung", "apple", "blackberry", "nokia"]
    }
  },
  mounted:function(){
    this.msg = localStorage.cli;
    this.msg = ++this.msg;
  },
  methods:{
    zalupa(event){
      alert("ss");
      alert(event.target.value);
      // alert(this.i);
    },
    countProducts: function(){
      this.$appName = ++this.$appName;
      alert(this.$appName);
      return this.$appName;
    },
    changeMessage(event) {
      this.message = event.target.value;
      this.$emit('messageChanged', this.message);
    },
    numberChanged(event) {
      this.i = event.target.name;
      this.displayActive = "block";
      this.$emit('numberChanged', this.displayActive);
      this.$emit('valueModal', this.i);
    },
  },
  components:{
  }
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
.shop-container
  // background: #b5f2d2
  font-family: Rowland
  padding:
     top: 3%
     // bottom: 1%
.inline-products
  display: flex
  width: 76%
  justify-content: space-between
  margin: 0 auto
  padding-bottom: 4%
@media screen and (max-width: 768px)
  .inline-products
    display: block
    width: 72%
@media screen and (max-width: 480px)
  .inline-products
    justify-content: center
    width: 62%
      padding-bottom: 0%
.double
  display: flex
  justify-content: space-between
  width: 46.5%
@media screen and (max-width: 768px)
  .double
    display: flex
    width: 98%
    justify-content: space-between
    margin: 0 auto
    padding-bottom: 4%
@media screen and (max-width: 480px)
   .double
     flex-direction: column
     justify-content: center
     padding-bottom: 0%
// .product:nth-child(1)
//   width: 50%
//   margin: 1%
// .product:nth-child(2)
//   width: 50%
//   margin: 1%
.product
  width: 40%
  margin: 1%
@media screen and (max-width: 480px)
  .product
    padding-bottom: 3%
.product-buy
  position: absolute
  margin: 0 auto
  width: 220px
  display: flex
  z-index: 2
  padding-top: 4%
.product-buy h4
  margin-left: 100px
  margin: 0 auto
  text-align: center
.buy
  position: relative

.product-img
  width: 18vw
  height: 23vw
  display: flex
  z-index: 1
.product-img img
  width: 18vw
  height: 23vw
  margin: 0 auto
.product-img img:hover
  width: 17vw
  height: 22vw
  transition: 0.5s
  filter: blur(0.8px)
@media screen and (max-width: 768px)
  .product-img
    width: 30vw
    height: 34vw
  .product-img img
    width: 29.2vw
    height: 34vw
  .product-img img:hover
    width: 29vw
    height: 33vw
@media screen and (max-width: 480px)
  .product-img
    width: 60vw
    height: 70vw
  .product-img img
    width: 60vw
    height: 70vw
  .product-img img:hover
    width: 59vw
    height: 69vw
.product-name
  margin:
    top: 1vw
    bottom: 2%
.product-name h4
  font-size: 1.8rem
  font-weight: 400
.product-price
  margin:
    top: 2%
    bottom: 2%
.product-price h5
  font-size: 1.4rem
  font-weight: 400
.product-button
  display: flex
  width: 98px
  margin: 0 auto
.product-button button
  border: 1px solid black
  background: white
  width: 100%
  height: 30px
  font-size: 0.9rem
.product-button button:hover
  background: #2f253e
  color: white
</style>
