<template>
  <div id="app">

    <myHeader />
    <myMain />
    <myFooter />
    <myFixedElements />

  </div>
</template>

<script>
import myHeader from './components/myHeader.vue';
import myMain from './components/myMain.vue';
import myFooter from './components/myFooter.vue';
import myFixedElements from './components/myFixedElements.vue';

export default {
  name: 'App',
  components: {
    myHeader,
    myMain,
    myFooter,
    myFixedElements
  }
}
</script>

<style lang="scss">
@import './assets/style/global';
@import './assets/style/utils';

</style>
