<script>

import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import HomePage from './components/HomePage.vue';
import AppReviews from './components/AppReviews.vue';
import AppProducts from './components/AppProducts.vue';
import AppFAQ from './components/AppFAQ.vue';
import AppInfo from './components/AppInfo.vue';
import Icons from './components/Icons.vue';

export default {

  components: {
    AppHeader,
    AppJumbo,
    HomePage,
    AppReviews,
    AppProducts,
    AppFAQ,
    AppInfo,
    Icons,
  }

}

</script>

<template>

  <!-- Include il componente delle icone -->
  <Icons></Icons>

  <AppHeader></AppHeader>

  <AppJumbo></AppJumbo>

  <HomePage></HomePage>

  <AppReviews></AppReviews>

  <AppProducts></AppProducts>

  <AppFAQ></AppFAQ>

  <AppInfo></AppInfo>

</template>

<style>



</style>