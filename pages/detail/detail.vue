<template>
  <view class="detail">
    <!-- 文章标题 -->
    <view class="title">接入标题的接口</view>
    <!-- 文章信息（作者和发布日期） -->
    <view class="info">
      <view class="author">编辑：接入编辑的接口</view>
      <view class="time">发布日期：接入发布日期的接口</view>
    </view>
    <!-- 文章内容 -->
    <view class="content">
      <rich-text>接入合适的文章内容部分的api接口</rich-text>
    </view>
    <!-- 声明信息 -->
    <view class="description">
      声明：本站的内容均采集与腾讯新闻，本站进行了内容采集不代表本站及作者观点，若有侵犯请及时联系管理员，谢谢您的支持。
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
  .detail {
    padding: 30rpx;

    .title {
      font-size: 46rpx;
      color: #333;
    }

    .info {
      background: #F6F6F6;
      padding: 20rpx;
      font-size: 25rpx;
      color: #666;
      display: flex;
      justify-content: space-between;
      margin: 40rpx 0;
    }

    .content {
      padding-bottom: 50rpx;
    }

    .description {
      background: #FEF0F0;
      font-size: 26rpx;
      padding: 20rpx;
      color: #F89898;
      line-height: 1.8em;
    }
  }
</style>