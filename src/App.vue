<script setup>

</script>

<template>
  <div class="wrapper">
    <div class="position">
      <span class="position__icon iconfont">&#xe7f1;</span>
      北京理工大学国防科技园2号楼10层
      <span class="position__notice iconfont">&#xe70a;</span>
    </div>
    <div class="search">
      <div class="search__icon iconfont">&#xe67d;</div>
      <span>山姆会员商店优惠商品</span>
    </div>
    <div class="banner">
      <img 
      src="http://www.dell-lee.com/imgs/vue3/banner.jpg" 
      class="banner__img"
      >
    </div>
  </div>
  <div class="docker">
    <div class="docker__item docker__item--active">
      <div class="iconfont">&#xe674;</div>
      <div class="docker__title">首页</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe826;</div>
      <div class="docker__title">购物车</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe713;</div>
      <div class="docker__title">订单</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe78b;</div>
      <div class="docker__title">我的</div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@import '@/style/mixins.scss';
@import '@/style/visible.scss';
.wrapper {
  position: fixed;
  top: 0;
  left: 0;
  bottom: .5rem;
  right: 0;
  padding: 0 .18rem;
  color: $content-fontcolor;
  .position {
    position: relative;
    padding: .16rem 0;
    padding-right: .24rem;
    @include ellipse;
    &__icon {
      font-size: .16rem;
      margin-right: .08rem;
    }
    &__notice {
      position: absolute;
      right: 0;
      top: .12rem;
      font-size: .2rem;
    }
  }
  .search  {
    vertical-align: middle;
    line-height: .32rem;
    background-color: #f5f5f5;
    border-radius: .16rem;
    font-size: .14rem;
    color: #b7b7b7;
    margin-bottom: 0.12rem;
    &__icon {
      display: inline-block;
      font-size: .16rem;
      padding-left: .16rem;
      padding-right: .12rem;
    }
  }
  .banner {
    height: 0;
    padding-bottom: 25.4%;
    overflow: hidden;
    &__img {
      width: 100%;
    }
  }
}
.docker {
  display: flex;
  position: fixed;
  left: 0;
  bottom: 0;
  height: .49rem;
  border-top: .01rem solid #f1f1f1;
  width: 100%;
  padding: 0 .18rem;
  box-sizing: border-box;
  color: $content-fontcolor;
  &__item {
    flex: 1;
    text-align: center;
    .iconfont {
      font-size: .18rem;
      margin-top: .07rem;
    }
    &--active {
      color: #1FA4FC;
    }
  }
  &__title  {
    font-size: .2rem;
    transform: scale(.5, .5);
    transform-origin: top center;
  }
}
</style>