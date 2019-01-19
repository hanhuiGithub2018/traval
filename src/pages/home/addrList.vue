<template>
    <ul class="clear addList">
       <li v-for="item in addrList" :key="item.id">
         <img :src="item.imgUrl">
         <p>{{item.disc}}</p>
       </li>
    </ul>
</template>

<script>
export default {
  name: 'HomeList',
  props: {
    addrList: Array
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
