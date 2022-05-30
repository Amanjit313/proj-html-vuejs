<template>
  <main>

    <myMainProducts />
    <myMainProcedure />

  </main>
</template>

<script>
import myMainProducts from './myMainProducts.vue';
import myMainProcedure from './myMainProcedure.vue';

export default {
  name: "myMain",
  components: {
    myMainProducts,
    myMainProcedure
  }
}
</script>

<style lang="scss" scoped>

</style>