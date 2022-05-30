<template>
  <main>

    <myMainProducts />
    <myMainProcedure />
    <myMainLocationsSharing />
    <myMainOrderShop />

  </main>
</template>

<script>
import myMainProducts from './myMainProducts.vue';
import myMainProcedure from './myMainProcedure.vue';
import myMainLocationsSharing from './myMainLocationsSharing.vue';
import myMainOrderShop from './myMainOrderShop.vue';

export default {
  name: "myMain",
  components: {
    myMainProducts,
    myMainProcedure,
    myMainLocationsSharing,
    myMainOrderShop
  }
}
</script>

<style lang="scss" scoped>

</style>