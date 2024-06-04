<template>
    <view>
      <u-navbar title="首页" @rightClick="rightClick" @leftClick="leftClick" :autoBack="false"> </u-navbar>
    </view>
  </template>
  
  <script>
  export default {
    data() {
      return {}
    },
    onLoad() {},
    methods: {
      rightClick() {
        console.log('rightClick')
      },
      leftClick() {
        console.log('leftClick')
      },
    },
  }
  </script>
  
  <style></style>
  