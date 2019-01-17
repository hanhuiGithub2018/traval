<template>
  <div class="wiper">
    <swiper :options="swiperOption" ref="mySwiper">
      <!-- slides -->
      <swiper-slide><img src="http://img1.qunarzz.com/piao/fusion/1811/31/da037478f37cf202.jpg_750x200_fe28d396.jpg"></swiper-slide>
      <swiper-slide><img src="http://img1.qunarzz.com/piao/fusion/1811/7c/8e5c4ab8ee8b7402.jpg_750x200_dd7a38dd.jpg"></swiper-slide>
      <swiper-slide><img src="http://img1.qunarzz.com/piao/fusion/1812/47/7be913b6e9c4bb02.jpg_750x200_ed626b8e.jpg"></swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data: function () {
    return {
      swiperOption: {
        loop: true,
        autoplay: true
      }
    }
  }
}
</script>

<style scoped>
  .wiper{
    width: 10rem;height: 2.6667rem;
  }
</style>
