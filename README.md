安装swiper。
  npm install --save swiper
父组件Home.vue：
导入数据
<template>
  <home-banner :listImg="listImg"></home-banner>
</template>
引入banner组件
<script>
  import Banner from './banner.vue'
  export default{
    data(){
      return {
        listImg:[
        {url:'./a.img'},
        {url:'./b.img'},
        {url:'./c.img'},
        {url:'./d.img'},
        ]
      }    
    },
    components:{
      'home-banner':Banner
    }
  }
</script>
