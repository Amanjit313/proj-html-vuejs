<template>
  <footer>

    <!-- Subscribe & Menu -->
    <div class="subscribe-menu">

      <!-- Footer Logo & Menu -->
      <div class="footer-logo-menu">
        <img src="../assets/img/avada-bakery-logo.png" alt="logo">
          <div class="menu">
            <ul>
              <li v-for="(options, index) in menu" :key="`menu-${index}`">
                <a :class="{active : options.isActive}" :href="options.href">{{options.select}}</a>
              </li>
            </ul>
            <i class="fa-solid fa-cart-shopping main-color"><span>0</span></i>
          </div>
      </div>
      <!-- /Footer Logo & Menu -->

      <!-- Subscribe -->
      <div class="subscribe">
        <h4>Subscribe to our Newsletter</h4>
        <div class="subscribe-button">
          <input type="email" placeholder="Enter email address*">
          <button class="btn-2"><span>Subscribe</span></button>
        </div>
      </div>
      <!-- /Subscribe -->

    </div>
    <!-- /Subscribe & Menu -->

    <!-- Copyright & Social -->
    <div class="copyright-social">
      <div class="copyright">&copy; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reversed | Powered by WordPress</div>
      <div class="social main-color">
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-facebook-f"></i>
        <i class="fa-brands fa-pinterest-p"></i>
      </div>
    </div>
    <!-- /Copyright & Social -->

    <!-- Chevron -->
    <div class="chevron">
      <i class="fa-solid fa-chevron-up"></i>
    </div>
    <!-- /Chevron -->

  </footer>
</template>

<script>
export default {
  name: "myFooter",

    data(){
    return{
      menu: [
        {
          select: "Shop",
          href: "#",
          isActive: false
        },
        {
          select: "About",
          href: "#",
          isActive: false
        },
        {
          select: "Gallery",
          href: "#",
          isActive: false
        },
        {
          select: "Locations",
          href: "#",
          isActive: false
        },
        {
          select: "Journal",
          href: "#",
          isActive: false
        },
        {
          select: "Contact",
          href: "#",
          isActive: false
        },
        {
          select: "Orders",
          href: "#",
          isActive: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

/* Subscribe & Menu */
.subscribe-menu{
  display: flex;
  justify-content: space-between;
}

/* Footer Logo & Menu */
.footer-logo-menu{
  margin-left: 60px;
  margin-top: 50px;
}

img{
  width: 9rem;
  margin-left: 10px;
  margin-bottom: 40px;
}

.menu{
  display: flex;
  align-items: center;
}

a{
  font-size: .95rem;
  margin-right: 40px;
  padding: 5px 0px;
}

.footer-logo-menu i{
  margin: 0px 10px;
  cursor: pointer;
}

.footer-logo-menu i span{
  background-color: rgba($color: #929295, $alpha: .3);
  padding: 5px 8px;
  border-radius: 50%;
  margin-left: 5px;
}

/* Subscribe */
.subscribe{
  margin-right: 60px;
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

input{
  padding: 6px 200px 6px 10px;
  border: 1px solid rgba($color: #929295, $alpha: .3);
  border-radius: 5px;
  margin-right: 10px;
}

h4{
  font-size: 1.2rem;
  color: #5b2ca2;
  margin-bottom: 40px;
  margin-top: 10px;
}

/* Copyright & Social */
.copyright-social{
  display: flex;
  justify-content: space-between;
  margin: 100px 60px 0px 60px;
}

.copyright{
  font-size: .75rem;
  color: #878589;
}

.social i{
  margin: 0px 15px;
  font-size: 1.1rem;
  cursor: pointer;
}

/* Chevron */
.chevron{
  color: white;
  margin-right: 50px;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.chevron i{
  padding: 10px 12px;
  background-color: rgba($color: #282d2c, $alpha: .9);
  border-radius: 5px;
}

</style>