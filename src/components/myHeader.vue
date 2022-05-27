<template>
  <header> <!-- Jumbotron -->

    <!-- Header Logo & Menu -->
    <div class="header-logo-menu">
      <img src="../assets/img/avada-bakery-logo.png" alt="logo">
      <div class="menu">
        <ul>
          <li v-for="(options, index) in menu" :key="`menu-${index}`">
            <a :class="{active : options.isActive}" :href="options.href">{{options.select}}</a>
          </li>
        </ul>
        <i class="fa-solid fa-cart-shopping"></i>
      </div>
    </div>
    <!-- /Header Logo & Menu -->

    <!-- Header Content -->
    <div class="w-90 center header-content">
      <div class="w-25">
        <p class="title">Fresh & tasty bakery every day</p>
        <h1 class="main-title">The Perfect Fresh Bread</h1>
        <p class="description">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Aliquam erat volutpat. Nullam quis saggittis nibh ac nulla id orci tempor.</p>
        <button class="btn-1"><span>Explore our products</span></button>
      </div>
    </div>
    <!-- /Header Content -->

  </header> <!-- /Jumbotron -->
</template>

<script>
export default {
  name: "myHeader",

  data(){
    return{
      menu: [
        {
          select: "Home",
          href: "#",
          isActive: true
        },
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
          select: "My Account",
          href: "#",
          isActive: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

header{
  height: 80vh;
  background-image: url('../assets/img/hero-header-bakery.jpg');
  background-size: cover;
}

/* Header Logo & Menu */
img{
  width: 11rem;
  padding: 0px 0px 0px 20px;
}

.header-logo-menu{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px 0px 0px;
}

.menu{
  display: flex;
  align-items: center;
}

a{
  font-size: .7rem;
  text-transform: uppercase;
  margin-right: 20px;
  padding: 5px 0px;
}

i{
  margin: 0px 20px;
}

.active{
  border-bottom: 2px solid #5b2ca2;
  width: 50%;
}

/* Header Content */
.header-content{
  display: flex;
  height: 80%;
  align-items: center;
}

p{
  color: #929295;
  margin: 20px 0px;
}

.title{
  text-transform: uppercase;
  font-size: .65rem;
}

.main-title{
  color: #5b2ca2;
  font-size: 3rem;
}

</style>