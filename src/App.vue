<script>

import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import HomePage from './components/HomePage.vue';
import AppReviews from './components/AppReviews.vue';
import AppProducts from './components/AppProducts.vue';
import AppFAQ from './components/AppFAQ.vue';
import AppInfo from './components/AppInfo.vue';
import Icons from './components/Icons.vue';
import ContactUs from './components/ContactUs.vue';

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
    ContactUs,
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

  <ContactUs></ContactUs>
  
</template>

<style>



</style>