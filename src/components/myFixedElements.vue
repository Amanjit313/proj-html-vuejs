<template>

  <!-- Fixed Element -->
  <div class="fixed-element">

  <!-- First Element -->
    <div class="first-element">
      <i class="fa-solid fa-cloud-arrow-up"></i>
      <p>Demos</p>
    </div>
  <!-- /First Element -->

  <!-- Second Element -->
    <div class="second-element">
      <!-- <h3>39</h3> -->
      <span>
        <h3>$</h3>
        <h2>39</h2>
      </span>
      <p>On Sale</p>
    </div>
  <!-- /Second Element -->

  </div>
  <!-- /Fixed Element -->

</template>

<script>

export default {
  name: "myFixedElements"
}
</script>

<style lang="scss" scoped>

.first-element{
  margin-top: 150px;
}

.second-element{
  margin-top: 220px;
}

.first-element,
.second-element{
  background-color: white;
  width: 60px;
  height: 60px;
  position: fixed;
  z-index: 999;
  top: 0;
  right: 0;
  margin-right: 10px;
  border-radius: 5px;
  box-shadow: 1px 1px 20px 5px rgba($color: #000000, $alpha: .2);
  cursor: pointer;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;

  &:hover{
    filter: brightness(95%);
  }
}

i{
  font-size: 1.4rem;
  color: #33475B;
  padding: 7px;
}

p{
  font-size: .9rem;
}

span{
  color: #64BC79;
  display: flex;
  justify-content: center;
}

span h2{
  margin-left: 1px;
  font-size: 2rem;
}

</style>