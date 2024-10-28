<template>
  <view class="user">
    <!-- 顶部栏显示图标和标题 -->
    <view class="top">
      <image src="../../static/images/history.png" mode=""></image>
      <view class="text">浏览历史</view>
    </view>
    <!-- 历史记录内容区域 -->
    <view class="content">
      <view class="row">
        用我给出的newsbox组件给出符合历史浏览条件的新闻列表
      </view>
    </view>

    <!-- 当没有浏览记录时显示的无数据提示 -->
    <view class="nohistory">
      <image src="../../static/images/nohis.png" mode="widthFix"></image>
      <view class="text">暂无浏览记录</view>
    </view>


  </view>
</template>

<script>
  export default {
    data() {
      return {

      }
    },
    methods: {

    }
  }
</script>

<style lang="scss">
  .user {
    .top {
      padding: 50rpx 0;
      background: #F8F8F8;
      color: #666;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      image {
        width: 150rpx;
        height: 150rpx;
      }

      .text {
        font-size: 38rpx;
        padding-top: 20rpx;
      }
    }

    .content {
      padding: 30rpx;

      .row {
        border-bottom: 1px dotted #efefef;
        padding: 20rpx 0;
      }
    }

    .nohistory {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      image {
        width: 450rpx;
      }

      .text {
        font-size: 26rpx;
        color: #888;
      }
    }
  }
</style>