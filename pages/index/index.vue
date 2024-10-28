<template>
  <view class="home">
    <!-- 导航栏 -->
    <scroll-view scroll-x class="navscroll">
      <view class="item">加入从api获得的分类名接口</view>
    </scroll-view>

    <!-- 新闻列表 -->
    <view class="content">
      <div class="row">
        用我给出的newsbox组件给出合适长度的新闻列表
      </div>
    </view>

    <!-- 无数据提示 -->前端已完成，无需添加任何代码
    <view class="nodata" v-if="!newsArr.length">
      <image src="../../static/images/nodata.png" mode="widthFix"></image>
    </view>

    <!-- 数据加载提示 -->前端已完成，无需添加任何代码
    <view class="loading" v-if="newsArr.length">
      <view v-if="loading==1">数据加载中...</view>
      <view v-if="loading==2">没有更多了~~</view>
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

<style lang="scss" scoped>
  .navscroll {
    height: 100rpx;
    background: #F7F8FA;
    white-space: nowrap;
    position: fixed;
    top: var(--window-top);
    left: 0;
    z-index: 10;

    /deep/ ::-webkit-scrollbar {
      width: 4px !important;
      height: 1px !important;
      overflow: auto !important;
      background: transparent !important;
      -webkit-appearance: auto !important;
      display: block;
    }

    .item {
      font-size: 40rpx;
      display: inline-block;
      line-height: 100rpx;
      padding: 0 30rpx;
      color: #333;

      &.active {
        color: #31C27C;
      }
    }
  }

  .content {
    padding: 30rpx;
    padding-top: 130rpx;

    .row {
      border-bottom: 1px dotted #efefef;
      padding: 20rpx 0;
    }
  }

  .nodata {
    display: flex;
    justify-content: center;

    image {
      width: 360rpx;
    }
  }

  .loading {
    text-align: center;
    font-size: 26rpx;
    color: #888;
    line-height: 2em;
  }
</style>