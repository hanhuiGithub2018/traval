<template>
  <div>
      <home-header :city="city"></home-header>
      <home-swiper></home-swiper>
      <home-list :addrList="addrList"></home-list>
      <home-detail :addrDetail="addrDetail"></home-detail>
  </div>
</template>

<script>
import HomeHeader from './header'
import HomeSwiper from './swiper'
import HomeList from './addrList'
import HomeDetail from './addrDetail'
import axios from 'axios'

export default {
  name: 'Home',
  data () {
    return {
      city: '',
      addrDetail: [],
      addrList: []
    }
  },
  components: {
    HomeSwiper, HomeHeader, HomeList, HomeDetail
  },
  methods: {
    getHomeInfo: function () {
      axios.get('/api/home.json').then(this.getHomeData)
    },
    getHomeData: function (res) {
      if (res.data.ret && res.data) {
        this.city = res.data.data.city
        this.addrList = res.data.data.addrList
        this.addrDetail = res.data.data.addrDetail
      }
    }
  },
  mounted: function () {
    this.getHomeInfo()
  }
}
</script>
