<template>
  <div class="container">
    <img class="child-image" src="http://admin.czhait.com/wwwroot/assets/svg/zk-classification.svg"></img>
    <x-icon name="zk-classification" link='/index'></x-icon>
    <zk-grid></zk-grid>
    <span>{{clientType}}</span>
  </div>
</template>

<script>
  // import api from '@/service/api/api'

  export default {
    config: {
      'navigationBarBackgroundColor': '#ffffff',
      'navigationBarTextStyle': 'black',
      'navigationBarTitleText': '微信接口功能演示',
      'backgroundColor': '#eeeeee',
      'backgroundTextStyle': true
    },
    data () {
      return {
        clientType: ''
      }
    },
    mounted () {
      this.ApiGet()
    },
    methods: {
      async  ApiGet () {
        // this.clientType = this.clientType()
        // var data = api.getNewsList()
        // console.info('fly', data)
      }
    }
  }
</script>

<style scoped lang="less">
</style>
