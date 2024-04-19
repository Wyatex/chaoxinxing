<template>
  <view>
    <view class="fixed left-0 top-0 right-0">
      <view class="w-full h-128rpx flex items-center justify-between">
        <view class="flex items-center">
          <view
            class="i-material-symbols-arrow-back-ios-rounded text-white text-60rpx ml-32rpx"
          ></view>
          <view
            class="bg-#00000033 flex items-center rounded-999"
            @click="onOpenHome"
          >
            <image
              src="/static/avatar.jpg"
              class="rounded-999 w-80rpx h-80rpx ml-8rpx my-8rpx"
            ></image>
            <view class="text-white ml-16rpx">
              <view class="text-32rpx">kaka新星</view>
              <view>9999人看过</view>
            </view>
            <view
              class="px-28rpx py-16rpx rounded-999 bg-#FB7196 text-white flex-center ml-16rpx mr-14rpx"
            >
              <view class="i-material-symbols-add"></view>
              <text class="text-30rpx">关注</text>
            </view>
          </view>
        </view>
        <view class="flex-center">
          <view class="px-32rpx py-28rpx rounded-999 bg-#00000033 text-white"
            >999+</view
          >
          <view
            class="i-material-symbols-more-vert text-white text-48rpx mx-8rpx"
          ></view>
        </view>
      </view>
      <view class="flex items-center justify-between mt-32rpx">
        <view class="flex-center">
          <view
            class="bg-#00000033 rounded-999 ml-48rpx py-8rpx px-16rpx flex-center"
          >
            <image src="/static/fire.png" class="w-26rpx h-26rpx"></image>
            <text class="text-white ml-4rpx">人气榜</text>
          </view>
          <view
            class="bg-#00000033 rounded-999 ml-16rpx py-8rpx px-16rpx flex-center"
          >
            <view
              class="i-icon-park-outline-ranking text-26rpx text-#FB7196"
            ></view>
            <text class="text-white ml-4rpx">虚拟主播榜第1名</text>
          </view>
        </view>
        <view class="flex-center rounded-l-999 bg-#00000033 py-8rpx pl-16rpx">
          <view class="i-uiw-appstore text-26rpx text-white"></view>
          <text class="text-white ml-8rpx">更多直播</text>
          <view
            class="i-material-symbols-arrow-forward-ios-rounded text-white text-24rpx mx-4rpx"
          ></view>
        </view>
      </view>
      <view class="flex justify-end mt-64rpx mr-16rpx">
        <view class="p-8rpx bg-#00000033 rounded-8rpx flex-center">
          <view class="text-white">
            <view>礼物星球</view>
            <view>暂未达成</view>
          </view>
          <image
            src="/static/gift-star.png"
            class="w-80rpx h-80rpx ml-16rpx"
          ></image>
        </view>
      </view>
    </view>
    <slot></slot>
    <view class="fixed bottom-0 left-0 right-0">
      <view class="w-full flex items-center px-32rpx py-16rpx gap-x-16rpx">
        <view
          class="w-80rpx h-80rpx rounded-999 relative bg-#00000066 flex-center"
        >
          <image src="/static/func.png" class="w-46rpx h-46rpx"></image>
          <view
            class="w-16rpx h-16rpx rounded-999 bg-#FC5D57 absolute right-0 top-0"
          ></view>
        </view>
        <view
          class="h-80rpx flex-1 flex items-center justify-between rounded-999 bg-#00000066"
        >
          <text class="text-#ddd ml-16rpx">等你发弹幕 ~ </text>
          <image
            src="/static/smile.png"
            class="w-60rpx h-60rpx mr-10rpx"
          ></image>
        </view>
        <view class="w-80rpx h-80rpx rounded-999 bg-#00000066 flex-center">
          <image src="/static/message.png" class="w-46rpx h-46rpx"></image>
        </view>
        <view class="w-80rpx h-80rpx rounded-999 bg-#00000066 flex-center">
          <image src="/static/rose.png" class="w-46rpx h-46rpx"></image>
        </view>
        <view class="w-80rpx h-80rpx rounded-999 bg-#00000066 flex-center">
          <image src="/static/gift.png" class="w-46rpx h-46rpx"></image>
        </view>
      </view>
    </view>
  </view>
</template>

<script setup lang="ts">
const onOpenHome = () => {
  window.open('https://space.bilibili.com/34283559')
}
</script>

<style scoped></style>
