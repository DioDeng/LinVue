<template>
  <section class="fixed-top" style="z-index: 1">
    <swiper
      :slidesPerView="1"
      :spaceBetween="30"
      :loop="true"
      :pagination="{
        clickable: true,
      }"
      :navigation="true"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide
        class="bgSet"
        :style="{
          'background-image':
            'url(' + require('@/assets/images/header-01.jpg') + ')',
        }"
      >
        <div>
          <h2 class="text-light mb-4">我們深信，服務-來自您的需求</h2>
          <h5 class="text-light mb-4">才 能 給 予 您 更 多 更 好</h5>
          <button class="btn btn-warning text-light p-3 h6">
            Service provided from your Needs
          </button>
        </div></swiper-slide
      >
      <swiper-slide
        class="bgSet"
        :style="{
          'background-image':
            'url(' + require('@/assets/images/header-02.jpg') + ')',
        }"
        >Slide 1</swiper-slide
      >
      <swiper-slide
        class="bgSet"
        :style="{
          'background-image':
            'url(' + require('@/assets/images/header-03.jpg') + ')',
        }"
        >Slide 1</swiper-slide
      >
    </swiper>
  </section>
</template>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;
  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.swiper {
  margin-left: auto;
  margin-right: auto;
}
.bgSet {
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  height:100vh;
}
</style>

<script>
// Import Swiper Vue.js components
// eslint-disable-next-line import/no-extraneous-dependencies
import { Swiper, SwiperSlide } from 'swiper/vue';
// import required modules
// eslint-disable-next-line import/no-extraneous-dependencies
import { Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
    };
  },
};
</script>
