<template>

  <!-- Procedure -->
  <div class="procedure w-80 center">

    <!-- Step 1 -->
    <div class="step-1">

      <img class="w-100" src="../assets/img/bakery-process-1.jpg" alt="bakery-process">

      <div class="step-1-title w-90 center">
        <h3 class="main-title-big-white w-40">Tell us what you have in mind</h3>
        <span class="number">01</span>
      </div>

      <div class="step-1-text w-90 center">
        <h3 class="title-lg w-25">Manual ingredients selection</h3>
        <p class="description-white w-25">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit pacerat, rutrum augue.</p>
      </div>

    </div>
    <!-- /Step 1 -->

    <div class="step-2-comments">
      <!-- Step 2 -->
      <div class="step-2 w-45">

        <img class="w-100" src="../assets/img/bakery-process-2.jpg" alt="bakery-process">

        <div class="step-2-title w-90 center">
          <h3 class="main-title-big-white">We start Baking</h3>
          <span class="number">02</span>
        </div>

        <div class="step-2-text w-90 center">
          <h3 class="title-lg w-50">Sweet & Delicious</h3>
          <p class="description-white w-50">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit pacerat.</p>
        </div>

      </div>
      <!-- /Step 2 -->

      <!-- Comments -->
      <div class="comments w-45">

        <div class="comments-text w-90 center">
          <h3 class="title">Dont just take our word for it</h3>
          <h3 class="main-title-big">"Finally found an alternative to the mass produced produtcs. Something that incorporates real organic ingredients, nutrient dense wellness while promoting sustainabilty and activity."</h3>
          <h3 class="title-no-up">Rachel Cooper, Founder</h3>
        </div>

      </div>
      <!-- Comments -->

    </div>

    <!-- Step 3 -->
    <div class="step-3">

      <img class="w-100" src="../assets/img/bakery-process-3.jpg" alt="bakery-process">

      <div class="step-3-title w-90 center">
        <h3 class="main-title-big-white w-40">Delivered to your home</h3>
        <span class="number">03</span>
      </div>

      <div class="step-3-text w-90 center">
        <h3 class="title-lg w-25">Baked to order & gift wrapped</h3>
        <p class="description-white w-25">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit pacerat, rutrum augue.</p>
      </div>

    </div>
    <!-- /Step 3 -->

  </div>
  <!-- Procedure -->

</template>

<script>

export default {
  name: "myMainProcedure",

}
</script>

<style lang="scss" scoped>

.procedure{
  margin-bottom: 100px;
}

.number{
  margin: 20px 0px;
  color: white;
  font-size: 5rem;
}

.description-white{
  margin-top: 20px;
}

.step-2-comments{
  display: flex;
  justify-content: space-between;
}

.step-1,
.step-2,
.comments,
.step-3{
  position: relative;
  margin-bottom: 25px;
}

.step-1 img,
.step-2 img,
.step-3 img{
  filter: brightness(60%);
  opacity: 95%;
}

.step-1-title,
.step-1-text,
.step-2-title,
.step-2-text,
.comments-text,
.step-3-title,
.step-3-text{
  display: flex;
  position: absolute;
  margin-left: 5%;
  margin-top: 30px;
}

.step-1-title,
.step-2-title,
.step-3-title{
  justify-content: space-between;
  top: 0;
}

.step-1-text,
.step-2-text,
.step-3-text{
  flex-direction: column;
  bottom: 0;
  margin-bottom: 40px;
}

/* Step 1 */
.step-1-text{
  align-items: flex-end;
}

/* Step 2 */
.step-2 img{
  height: 700px;
}

.step-2-text{
  align-items: flex-start;
}

/* Comments */
.comments{
  height: 700px;
  background-color: rgba($color: #e9dedc, $alpha: .5);
  display: flex;
  align-items: center;
}

.comments-text{
  flex-direction: column;
}

.main-title-big{
  margin: 40px 0px;
}

</style>