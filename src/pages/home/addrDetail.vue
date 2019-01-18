<template>
  <div class="bg-w mgt-20">
    <h3 class="title">热门推荐</h3>
    <ul>
      <li class="detail" v-for="item in addrList" :key="item.id">
        <div class="left"><img :src="item.imgUrl"></div>
        <div class="right">
          <h5 class="color-dg mgt-20 fs-30">{{item.title}}</h5>
          <div class="mgt-10"><span class="color-fo fs-30 mgr-30">{{item.star}}</span><span>{{item.talk}}</span></div>
          <div class="mgt-10">&yen; <span class="color-o fs-40">{{item.money}}</span> 起</div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
let addrList = [
  {
    id: '0001', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0002', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0003', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0004', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0005', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0006', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  },
  {
    id: '0007', imgUrl: '../../../static/images/10.jpg', title: '温泉假日酒店', star: '★★★★★', talk: '65条评论', money: '40'
  }
]
export default {
  name: 'HomeDetail',
  data: function () {
    return {
      addrList
    }
  }
}
</script>

<style scoped>
  .title{padding: .2667rem;font-size: .38rem}
  .detail{
    width: 100%;height:auto;margin-bottom: .2667rem;padding: 0 .2667rem;
    display: -webkit-box;display: flex;
  }
  .left{
    width: 2.667rem;height: 2.667rem;
  }
  .right{
    padding-left: .2667rem;
    flex-grow: 1;
  }
</style>
