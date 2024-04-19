<template>
  <layout>
    <view class="bg w-100vw h-100vh">
      <view> </view>
      <view
        v-if="!play"
        class="fixed left-1/2 top-1/2 -translate-1/2 i-ph-play-duotone text-120rpx"
        @click="onPlay"
      ></view>
    </view>
  </layout>
</template>

<script setup lang="ts">
import { onPullDownRefresh } from '@dcloudio/uni-app'

const play = ref(false)

const onPlay = () => {
  document.querySelector('audio').play()
  play.value = true
}
onPullDownRefresh(() => {
  uni.showToast({
    title: '已经到顶了~💗',
    icon: 'none'
  })
  setTimeout(() => {
    uni.stopPullDownRefresh()
  }, 10)
})
</script>

<script lang="ts">
export default {}
</script>

<style scoped>
.bg {
  background: url('/static/bg.jpg');
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
}
</style>
