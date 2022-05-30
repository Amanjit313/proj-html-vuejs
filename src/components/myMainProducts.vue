<template>

    <!-- Products -->
    <div class="products w-80 center">

      <!-- Shopping -->
      <div class="shopping">

        <div class="shopping-text w-400">
          <p class="title">Our products</p>
          <h3 class="main-title-small">All our delectable pastries are backed fresh in our Kitchen very morning, and are made with all-natural, all organic ingredients.</h3>
          <button class="btn-2"><span>Start Shopping</span></button>
        </div>

        <div class="shopping-products">
          <img class="s-first-img" src="../assets/img/choco-chip-cookies-400x510.jpg" alt="products">
          <img class="s-second-img" src="../assets/img/strawberry-jam-cookies-400x510.jpg" alt="products">
          <div class="s-first-selector">
            <i class="fa-solid fa-chevron-left"></i>
          </div>
          <div class="s-second-selector">
            <i class="fa-solid fa-chevron-right"></i>
          </div>
        </div>

      </div>
      <!-- /Shopping -->

      <!-- Corporate Weddings -->
      <div class="corporate-weddings">

        <div class="corporate-weddings-text">
          <p class="title">Corporate & weddings</p>
          <h3 class="main-title-small">Baking Special Moments</h3>
        </div>

        <!-- Corporate Weddings Img-->
        <div class="corporate-weddings-img">

          <div class="cp-visible-corporate">

            <img class="cp-img-visible-corporate" src="../assets/img/corporate-bg.jpg" alt="corporate-visible">

            <img class="cp-img-hover-corporate" src="../assets/img/corporate-hover-bg.jpg" alt="corporate-hover">

            <div class="corporate-weddings-text-corporate">
              <p class="title-white">International Bakery</p>
              <h3 class="main-title-small-white">Corporate Events</h3>
              <button class="btn-2"><span>Explore more</span></button>
            </div>

          </div>

          <div class="cp-visible-wedding">

            <img class="cp-img-visible-wedding" src="../assets/img/wedding-bg.jpg" alt="wedding-visible">
            
            <img class="cp-img-hover-wedding" src="../assets/img/wedding-hover-bg.jpg" alt="wedding-hover">

            <div class="corporate-weddings-text-weddings">
              <p class="title-white">Private Dining Hall</p>
              <h3 class="main-title-small-white">Weddings & Parties</h3>
              <button class="btn-2"><span>Explore more</span></button>
            </div>

          </div>

        </div>
        <!-- /Corporate Weddings Img-->

      </div>
      <!-- /Corporate Weddings -->

      <!-- All Products -->
      <div class="all-products">

        <div class="all-products-text w-350">
          <h3 class="main-title-small">Find a freshly baked product perfetct for you</h3>
          <p class="description">Integer a nibh vitae ex porttitor rutrum et ut velit. Etiam ac felis at leo feugiat placerat. Sed ac nulla id orci tempor convallis sed.</p>
          <button class="btn-2"><span>Shop All Products</span></button>
        </div>

        <div class="product-cards">

          <div class="product-singol-card main-color" v-for="(card, index) in productCards" :key="`productCards-${index}`">
            <img :src="card.img" alt="product-card" class="product-img">
            <h5>{{card.product}}</h5>
            <p>{{card.price}}</p>
          </div>
          
          <div class="s-first-selector-2">
            <i class="fa-solid fa-chevron-left"></i>
          </div>
          <div class="s-second-selector-2">
            <i class="fa-solid fa-chevron-right"></i>
          </div>

        </div>

      </div>
      <!-- /All Products -->

    </div>
    <!-- /Products -->

</template>

<script>
export default {
  name: "myMainProducts",

  data(){
    return{
      productCards: [
        {
          img: require('../assets/img/choco-chip-cookies-235x300.jpg'),
          product: "Choco Chip Cookies",
          price: "$19.00 - $39.00"
        },
        {
          img: require('../assets/img/strawberry-jam-cookies-235x300.jpg'),
          product: "Strawberry Jam Cookies",
          price: "$24.00 - $62.00"
        },
        {
          img: require('../assets/img/strawberry-donut-200x255.jpg'),
          product: "Strawberry Donut",
          price: "$24.00 - $42.00"
        },
        {
          img: require('../assets/img/perfect-macarons-200x255.jpg'),
          product: "Perfect Macarons",
          price: "$18.00 - $52.00"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

.products{
  margin-bottom: 100px;
}

/* Shopping */
.shopping{
  display: flex;
  justify-content: space-between;
  margin-bottom: 15vh;
}

.shopping-text button{
  margin-top: 30px;
}

.shopping-products{
  display: flex;
  position: relative;
}

.shopping-products img:nth-child(2){
  margin-left: 50px;
}

.s-first-selector{
  position: absolute;
  bottom: 240px;
  left: 0;
}

.s-second-selector{
  position: absolute;
  bottom: 240px;
  right: 0;
}

.shopping-products i,
.all-products i{
  padding: 20px 10px;
  background-color: rgba($color: #5b2ca2, $alpha: .4);
  color: white;
  cursor: pointer;

  &:hover{
    background-color: rgba($color: #5b2ca2, $alpha: .8);
  }
}

/* Corporate Weddings */
.corporate-weddings-text{
  text-align: center;
}

.corporate-weddings-img{
  display: flex;
  justify-content: space-between;
}

.corporate-weddings-img img{
  width: 45rem;
  margin-top: 25px;
}

.cp-visible-corporate,
.cp-visible-wedding{
  position: relative;
}

.cp-img-visible-corporate,
.cp-img-visible-wedding{
  position: relative;
  display: inline-block;
}

.cp-img-hover-corporate{
  position: absolute;
  top: 0;
  left: 0;
  display: none;
}

.cp-img-hover-wedding{
  position: absolute;
  top: 0;
  right: 0;
  display: none;
}

.cp-visible-corporate:hover .cp-img-hover-corporate,
.cp-visible-wedding:hover .cp-img-hover-wedding,
.cp-visible-corporate:hover .corporate-weddings-text-corporate,
.cp-visible-wedding:hover .corporate-weddings-text-weddings{
  display: inline;
}

.corporate-weddings-text-corporate,
.corporate-weddings-text-weddings{
  position: absolute;
  text-align: center;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: none;
}

/* All Products */
.all-products{
  display: flex;
  margin-top: 100px;
  text-align: center;
  justify-content: space-between;
  align-items: center;
}

.product-cards{
  display: flex;
}

.product-singol-card h5{
  margin: 10px 0px;
  font-size: 1.2rem;
}

.product-singol-card p{
  font-size: .9rem;
}

.product-cards{
  position: relative;
}

/* .product-cards :nth-child(2) img,
.product-cards :nth-child(3) img,
.product-cards :nth-child(4) img{
  margin-left: 20px;
} */

.s-first-selector-2{
  position: absolute;
  bottom: 50%;
  left: 0;
}

.s-second-selector-2{
  position: absolute;
  bottom: 50%;
  right: 0;
}

.product-img{
  width: 235px;
  height: 300px;
}

</style>