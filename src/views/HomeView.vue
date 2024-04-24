<template>
  <section>
    <header style="height: 100vh">
      <Carousel />
    </header>
    <main class="bg-light sticky-top">
      <Content />
      <Service />
    </main>
  </section>
</template>

<script>
import Carousel from '@/components/home/CarouselModel.vue';
import Content from '@/components/home/ContentModel.vue';
import Service from '@/components/home/ServiceModel.vue';

export default {
  name: 'HomeView',
  components: {
    Carousel,
    Content,
    Service,
  },
};
</script>
