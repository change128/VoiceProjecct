<template>
  <div>
    <div class="voice_image_wrapper">
     <!-- 
     voice 组件 props 接收一个 isActive 
     isActive===true 时加一个 active 类名 即可激活动效
     一个 hr 表示一个音浪 
     scaleY 纵向拉伸
     animation-delay 延迟播放动效
    -->
      <div class="voice_image">
        <hr class="hr1" v-bind:class="{ active: isActive }" />
        <hr class="hr2" v-bind:class="{ active: isActive }" />
        <hr class="hr3" v-bind:class="{ active: isActive }" />
        <hr class="hr4" v-bind:class="{ active: isActive }" />
        <hr class="hr5" v-bind:class="{ active: isActive }" />
        <hr class="hr6" v-bind:class="{ active: isActive }" />
        <hr class="hr7" v-bind:class="{ active: isActive }" />
        <hr class="hr8" v-bind:class="{ active: isActive }" />
        <hr class="hr9" v-bind:class="{ active: isActive }" />
        <hr class="hr10" v-bind:class="{ active: isActive }" />
        <hr class="hr11" v-bind:class="{ active: isActive }" />
        <hr class="hr12" v-bind:class="{ active: isActive }" />
        <hr class="hr13" v-bind:class="{ active: isActive }" />
        <hr class="hr14" v-bind:class="{ active: isActive }" />
        <hr class="hr15" v-bind:class="{ active: isActive }" />
        <hr class="hr16" v-bind:class="{ active: isActive }" />
        <hr class="hr17" v-bind:class="{ active: isActive }" />
        <hr class="hr18" v-bind:class="{ active: isActive }" />
        <hr class="hr19" v-bind:class="{ active: isActive }" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "",
  components: {},
  props:['isActive'],
  data() {
    return {
    };
  },
  methods: {
    changeFirstColor() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style lang="scss">
.active {
  animation:ani 0.2s  ease-in-out;
  animation-iteration-count:infinite;
  animation-direction:alternate;
}
.voice_image_wrapper {
  height: 100px;
  .voice_image {
    width: 300px;
    height:100px;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0 20px;
    background-color: #f8f8f8;
    hr {
    background-color:#4e95ff;
    width:5px;
    height:15px;
    display:inline-block;
    border:none;
    }
    .hr1{
    animation-delay:-1s;
    }
    .hr2{
    animation-delay:-0.9s;
    }
    .hr3{
    animation-delay:-0.8s;
    }
    .hr4{
    animation-delay:-0.7s;
    }
    .hr5{
    animation-delay:-0.6s;
    }
    .hr6{
    animation-delay:-0.5s;
    }
    .hr7{
    animation-delay:-0.4s;
    }
    .hr8{
    animation-delay:-0.3s;
    }
    .hr9{
    animation-delay:-0.2s;
    }
    .hr10{
    animation-delay:-0.1s;
    }
    .hr11{
    animation-delay:-1s;
    }
    .hr12{
    animation-delay:-0.9s;
    }
     .hr13{
    animation-delay:-0.8s;
    }
     .hr14{
    animation-delay:-0.7s;
    }
     .hr15{
    animation-delay:-0.6s;
    }
     .hr16{
    animation-delay:-0.5s;
    }
     .hr17{
    animation-delay:-0.4s;
    }
     .hr18{
    animation-delay:-0.3s;
    }
     .hr19{
    animation-delay:-0.2s;
    }
  }
}
@keyframes ani{
from {transform:scaleY(1);}
to {transform:scaleY(4);}

}
</style>
