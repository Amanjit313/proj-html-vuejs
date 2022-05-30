<template>

  <!-- Locations & Sharing -->
  <div class="locations-sharing w-80 center">

    <!-- Locations -->
    <div class="locations">

      <!-- Locations Title -->
      <div class="locations-title">
          <p class="title">Locations</p>
          <h3 class="main-title-small">Visit our Bakeries</h3>
      </div>
      <!-- /Locations Title -->

      <!-- Locations Info Box -->
      <div class="locations-info-box">

        <div class="locations-new-york">

          <img src="../assets/img/new-york-bk-800x530.jpg" alt="locations-new-york">

          <div class="locations-new-york-text w-80 center">

            <h3 class="main-title-small">New York</h3>

            <div class="locations-info">

              <div class="call-us">
                <p class="title">Call us</p>
                <p class="locations-details">1.800.458.566</p>
              </div>

              <div class="open-time">
                <p class="title">Open all week</p>
                <p class="locations-details">9.00 AM - 6:00 PM</p>
              </div>

              <div class="map">
                <button class="btn-1"><span>View Map</span></button>
              </div>

            </div>

          </div>

        </div>

        <div class="locations-london">
          <img src="../assets/img/london-bk-800x530.jpg" alt="locations-london">

          <div class="locations-london-text w-80 center">

            <h3 class="main-title-small">London</h3>

            <div class="locations-info">

              <div class="call-us">
                <p class="title">Call us</p>
                <p class="locations-details">1.800.458.566</p>
              </div>

              <div class="open-time">
                <p class="title">Open all week</p>
                <p class="locations-details">9.00 AM - 6:00 PM</p>
              </div>

              <div class="map">
                <button class="btn-1"><span>View Map</span></button>
              </div>

            </div>

          </div>

        </div>

      </div>
      <!-- /Locations Info Box -->

    </div>
    <!-- /Locations -->

    <!-- Sharing -->
    <div class="sharing">

      <img src="../assets/img/social-1.jpg" alt="sharing-photos" class="upper-img">

      <div class="follow-us">
          <p class="title">Made for sharing</p>
          <h3 class="main-title-small">Let's stay in touch</h3>
          <button class="btn-2">
            <span>
              <i class="fa-brands fa-instagram"></i>
              Follow us
            </span>
          </button>
      </div>

      <img src="../assets/img/social-2.jpg" alt="sharing-photos" class="upper-img">

      <img src="../assets/img/social-3.jpg" alt="sharing-photos" class="lower-img">

      <img src="../assets/img/social-4.jpg" alt="sharing-photos" class="lower-img costum-spacing-1">

      <img src="../assets/img/social-5.jpg" alt="sharing-photos" class="lower-img costum-spacing-2">

      <img src="../assets/img/social-6.jpg" alt="sharing-photos" class="lower-img">

    </div>
    <!-- /Sharing -->

  </div>

</template>

<script>
export default {
  name: "locations-sharing"
}
</script>

<style lang="scss" scoped>

/* Locations */
.locations{
  margin-bottom: 100px;
}

.locations-title{
  text-align: center;
  margin-bottom: 40px;
}

.locations-info-box{
  display: flex;
}

.locations-info-box img{
  width: 100%;
}

.locations-new-york{
  height: 70vh;
  background-color: rgba($color: #0a5e6c, $alpha: 0.1);
}

.locations-new-york-text{
  height: 16vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.locations-london{
  height: 70vh;
  background-color: rgba($color: #f0caa1, $alpha: 0.2);
}

.locations-london-text{
  height: 16vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.locations-info{
  display: flex;
  justify-content: space-between;
  width: 100%;
  text-align: center;
}

.locations-details{
  font-size: .9rem;
  margin-top: 10px;
  color: rgba($color: black, $alpha: .7);
}

/* Sharing */
.sharing{
  display: flex;
  flex-wrap: wrap;
}

.upper-img{
  width: 37vh;
  height: 400px;
}

.lower-img{
  width: calc(92.5% / 4);
  height: 350px;
  margin-top: 2.5%;
}

.follow-us{
  width: 77.4vh;
  height: 400px;
  background-color: rgba($color: #bda2f3, $alpha: .1);
  margin: 0px 2.5%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.costum-spacing-1{
  margin-right: 2.5%;
  margin-left: 2.5%;
}

.costum-spacing-2{
  margin-right: 2.5%;
}

.follow-us span i{
  margin-right: 5px;
}

</style>