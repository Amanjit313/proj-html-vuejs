<template>
  <main>

    <myMainProducts />
    <myMainProcedure />
    <myMainLocationsSharing />

  </main>
</template>

<script>
import myMainProducts from './myMainProducts.vue';
import myMainProcedure from './myMainProcedure.vue';
import myMainLocationsSharing from './myMainLocationsSharing.vue';

export default {
  name: "myMain",
  components: {
    myMainProducts,
    myMainProcedure,
    myMainLocationsSharing
  }
}
</script>

<style lang="scss" scoped>

</style>