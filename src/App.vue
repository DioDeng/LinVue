<template>
  <Navbar class="fixed-top" />
  <router-view />
  <Footer class="" />
</template>

<style lang="scss">
@import '@/assets/stylesheets/all';
</style>

<script>
import Navbar from '@/components/layout/NavbarModel.vue';
import Footer from '@/components/layout/FooterModel.vue';

export default {
  components: { Navbar, Footer },
};
</script>
