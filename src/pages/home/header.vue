<template>
  <div class="header">
    <a href="#" class="arrow-back"></a>
    <input type="text" class="search" placeholder="输入城市/美食/旅游景点">
    <a href="#" class="position">三亚</a>
  </div>
</template>

<script>
export default {
  name: 'HoneHeader'
}
</script>

<style scoped>
  .header{
    width: 100%;height: 1.1733rem;line-height: 1.1733rem;padding: 0 .2667rem;
    font-size: .32rem;color: #fff;background: #01B5CD;
    display: -webkit-flex;display: flex;
  }
  .arrow-back{
    width: .667rem;height: 1.17333rem;display: block;
    background: url('../../assets/images/arrow-back.png') no-repeat center center;
    background-size: 0.2267rem auto;
  }
  .search{
    padding: 0 .993rem 0 .2667rem;margin: .14rem;border: none;border-radius: 4px;font-size: .32rem;
    background: #fff url("../../assets/images/icon-search-nor.png") no-repeat 95% center;
    background-size: .4rem;
    flex-grow: 1;
  }
  .position{
    width: 1.6rem;text-align: center;
    background: url("../../assets/images/tangle-down.png") no-repeat right center;
    background-size: .32rem;
  }
</style>
