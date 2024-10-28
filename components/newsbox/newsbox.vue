<template>
  <view class="newsbox">
    <view class="pic">
      接入合适的后端图片api接口
    </view>
    <view class="text">
      <view class="title">
        接入合适的后端标题api接口
      </view>
      <view class="info">
        作者、浏览量后端的api接口
      </view>
      <view class="info">
        <text>浏览时间：（浏览时间后端api接口）</text>
      </view>
    </view>
  </view>
</template>

<script>
  export default {
    name: "newsbox",
    props: {
      item: {
        type: Object,
        default () {
          return {
            title: "组件内默认的标题",
            author: "计科2203班",
            hits: 2024,
            picurl: "../../static/images/nopic.jpg"
          }
        }
      }
    },
    data() {
      return {

      };
    }
  }
</script>

<style lang="scss">
  .newsbox {
    display: flex;

    .pic {
      width: 230rpx;
      height: 160rpx;

      image {
        width: 100%;
        height: 100%;
      }
    }

    .text {
      flex: 1;
      padding-left: 20rpx;
      display: flex;
      flex-direction: column;
      justify-content: space-between;

      .title {
        font-size: 36rpx;
        color: #333;
        text-overflow: -o-ellipsis-lastline;
        overflow: hidden; //溢出内容隐藏
        text-overflow: ellipsis; //文本溢出部分用省略号表示
        display: -webkit-box; //特别显示模式
        -webkit-line-clamp: 2; //行数
        line-clamp: 2;
        -webkit-box-orient: vertical; //盒子中内容竖直排列			
      }

      .info {
        font-size: 26rpx;
        color: #999;

        text {
          padding-right: 30rpx;
        }
      }
    }
  }
</style>