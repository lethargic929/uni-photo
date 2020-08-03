<template>
  <view class="content">
    <navigator
      url="navigate/navigate?title=navigate"
      hover-class="navigator-hover"
      class="search"
    >
     <view class="wrap">
       <button><icon type="search"  size="24"/>搜索</button>
     </view>
    </navigator>
    <swiper
      class="swiper"
      :indicator-dots="indicatorDots"
      :autoplay="autoplay"
      :interval="interval"
      :duration="duration"
    >
      <swiper-item>
        <view class="swiper-item uni-bg-red">
          <image  :mode="aspectFit" src="../static/uploads/banner1.png"></image>
        </view>
      </swiper-item>
    </swiper>
    <view class="nav">12</view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
};
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  box-sizing: border-box;
}
.search {
  width: 750rpx;
  height: 80rpx;
  background-color: #ea4450;
  padding: 15rpx;
}
.wrap button {
  height: 66rpx;
  line-height: 66rpx;
  background-color: #fff;
  margin: 10rpx 25rpx;
}
.wrap button icon {
  line-height: 66rpx;
  padding-right: 10rpx;
}
.swiper {
  width: 750rpx;
  height: 340rpx;
  background-color: pink;
}
.nav {
  width: 750rpx;
  height: 80rpx;
}
</style>
