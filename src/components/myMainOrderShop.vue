<template>

  <!-- Order Shop -->
  <div class="order-shop">
    <img src="../assets/img/call-to-action-bg.jpg" alt="order-shop-photo">
    <div class="order-shop-text w-60 center">
      <p class="title-lg">Try our seasonal products</p>
      <h3 class="main-title-big-white w-55">Order for pick-up or delivery to your home</h3>
      <button class="btn-1">
        <span>
          Shop now
        </span>
      </button>
    </div>
  </div>
  <!-- /Order Shop -->

</template>

<script>
export default {
  name: "myMainOrderShop"
}
</script>

<style lang="scss" scoped>

/* Order Shop */
.order-shop{
  position: relative;
}

.order-shop img{
  width: 100%;
  height: 550px;
}

.order-shop-text{
  position: absolute;
  top: 0;
  margin-left: 20%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}

.order-shop-text h3{
  margin-bottom: 50px;
}

</style>