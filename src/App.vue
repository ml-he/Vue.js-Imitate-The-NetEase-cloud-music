<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" @click="getWangyi"> -->
    <!-- <nav class="nav-wrapper">
      <div class="nav-left">
        <i class="login"></i>
      </div>
      <ul class="nav-center">
        <router-link tag="div" replace to="/home" :class="{changeFont:isTouch,font:isActive}" @touchstart.native="touch" @touchend.native='touchEnd'>
        <div class="cover" :class="{active:isLeave,bgc:isTouch}" ></div>我的</router-link>
        <router-link tag="div" replace to="/find" :class="{changeFont:isTouch,font:isActive}" @touchstart.native="touch" @touchend.native='touchEnd'>
        <div class="cover" :class="{active:isLeave,bgc:isTouch}" ></div>发现</router-link>
        
        
       
      </ul>
      <div class="nav-right">
        <router-link to="/search" >搜索</router-link>
      </div>
    </nav>-->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" @click.native="getSong"/> -->

    <keep-alive>
      <router-view></router-view>
    </keep-alive>
    <bottom-bar></bottom-bar>
  </div>
</template>

<script>
import Main from 'views/Main'
import Swipers from 'components/content/swiper.vue'

import BottomBar from 'components/content/player/BottomBar'
export default {
  components: {
    Swipers,
    BottomBar
  }
}
</script>

<style scoped>
.tab-bar {
  position: relative;
  top: -1px;
}
</style>
