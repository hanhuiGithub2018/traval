<template>
    <ul class="clear addList">
       <li v-for="item in addList" :key="item.id">
         <img :src="item.imgUrl">
         <p>{{item.disc}}</p>
       </li>
    </ul>
</template>

<script>
let addList = [
  {
    id: 1, disc: '景点门票', imgUrl: '../../../static/images/1.png'
  }, {
    id: 2, disc: '室内场馆', imgUrl: '../../../static/images/2.png'
  }, {
    id: 3, disc: '重庆必游', imgUrl: '../../../static/images/3.png'
  }, {
    id: 4, disc: '峨眉山', imgUrl: '../../../static/images/4.png'
  }, {
    id: 5, disc: '一日游', imgUrl: '../../../static/images/5.png'
  }, {
    id: 6, disc: '两江夜游', imgUrl: '../../../static/images/6.png'
  }, {
    id: 7, disc: '神秘山', imgUrl: '../../../static/images/7.png'
  }, {
    id: 8, disc: '泡温泉', imgUrl: '../../../static/images/8.png'
  }
]
export default {
  name: 'HomeList',
  data: function () {
    return {
      addList
    }
  }
}
</script>

<style scoped>
  .addList li{
    width: 2.5rem;height: 2.5rem;padding: .2667rem;float: left;text-align: center;font-size: .32rem;
    background: #fff;
  }
  .addList li img{
    width: 1.4rem;margin-bottom: .1333rem;
  }
</style>
