<template>
    <div id="home">
      <test></test>
      <slide :msg.sync="aa"></slide>  <!--.sync双向绑定-->
      <span>测试父子双向绑定：{{aa}}</span>
      <div class="home-list">
        <h2 class="home-title">我是薛之谦，我的梦想是世界和平...</h2>
        <p class="home-detail">我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...</p>
      </div>
      <div class="home-list">
        <h2 class="home-title">我是薛之谦，我的梦想是世界和平...</h2>
        <p class="home-detail">我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...</p>
      </div>
      <div class="home-list">
        <h2 class="home-title">我是薛之谦，我的梦想是世界和平...</h2>
        <p class="home-detail">我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...我是薛之谦，我的梦想是世界和平...</p>
      </div>
    </div>
</template>
<script>
    import test from './nav.vue'
    import slide from './slide.vue'
    export default{
        data(){
            return {
              aa: '我是props传递过来的数据'
            }
        },
        components: {
          test, slide
        }
    }
</script>

<style>
  .img-box {
    width: 100%;
  }

  .img-box img {
    height: 416px;
    width: 100%;
  }

  .home-list {
    border-bottom: 1px solid #e8e8e8;
  }

  .home-list .home-title {
    margin: 30px 0 15px;
  }

  .home-list .home-detail {
    margin-bottom: 30px;
  }
</style>
