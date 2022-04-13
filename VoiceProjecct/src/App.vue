<template>
<div>
   <!-- 实例代码 -->
    <button @touchstart="speakFn" @touchend="speakFn">点击</button>
    <!-- 音频组件 props传入一个 isActive Boolean true 播放动画 false 暂停动画 -->
  <voice v-bind:isActive="isActive"></voice>
  </div>
</template>

<script>
import Voice from "./components/Voice.vue";
export default {
  data() {
    return {
    // isActive Boolean true 播放动画 false 暂停动画
      isActive: false,
    };
  },
  methods: {
  // 语音函数
    speakFn() {
      this.isActive = !this.isActive;
    },
  },
  components: {
    Voice,
  },
};
</script>
