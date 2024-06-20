<script>

import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import HomePage from './components/HomePage.vue';
import AppReviews from './components/AppReviews.vue';

export default {

  components: {
    AppHeader,
    AppJumbo,
    HomePage,
    AppReviews,
  }

}

</script>

<template>

  <AppHeader></AppHeader>

  <AppJumbo></AppJumbo>

  <HomePage></HomePage>

  <AppReviews></AppReviews>

</template>

<style>



</style>