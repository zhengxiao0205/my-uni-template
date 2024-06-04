<template>
  <view>
    <u-navbar title="我的" @rightClick="rightClick" @leftClick="leftClick" :autoBack="false"> </u-navbar>
  </view>
</template>

<script>
import { getList, updateData } from '@/api/demo'
export default {
  data() {
    return {}
  },
  onLoad() {
    getList().then((res) => {
      console.log(res)
    })
  },
  methods: {
    rightClick() {
      console.log('right click')
    },
    leftClick() {
      updateData({ name: 'new name' }).then((res) => {
        console.log(res)
      })
    },
  },
}
</script>

<style></style>
