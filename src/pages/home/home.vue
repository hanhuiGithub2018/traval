<template>
  <div>
      <home-header></home-header>
      <home-swiper></home-swiper>
      <home-list></home-list>
      <home-detail></home-detail>
  </div>
</template>

<script>
import HomeHeader from './header'
import HomeSwiper from './swiper'
import HomeList from './addrList'
import HomeDetail from './addrDetail'

export default {
  name: 'Home',
  components: {
    HomeSwiper, HomeHeader, HomeList, HomeDetail
  }
}
</script>
