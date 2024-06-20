<script>

import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import HomePage from './components/HomePage.vue';
import AppReviews from './components/AppReviews.vue';
import AppProducts from './components/AppProducts.vue';
import AppFAQ from './components/AppFAQ.vue';

export default {

  components: {
    AppHeader,
    AppJumbo,
    HomePage,
    AppReviews,
    AppProducts,
    AppFAQ,
  }

}

</script>

<template>

  <AppHeader></AppHeader>

  <AppJumbo></AppJumbo>

  <HomePage></HomePage>

  <AppReviews></AppReviews>

  <AppProducts></AppProducts>

  <AppFAQ></AppFAQ>

</template>

<style>



</style>