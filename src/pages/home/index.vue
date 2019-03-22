<template>
  <div id='home'>
    <div class="home-banner">
      <swiper autoplay>
        <swiper-item  v-for='item in imgUrls' :key="item">
          <image  :src="item" class="slide-image" width="355" height="150" />
        </swiper-item>
      </swiper>
    </div>
    <div class="home-cont">
      <div class="home-cont-titile">这是title</div>
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      imgUrls: [
        'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640',
        'https://images.unsplash.com/photo-1551214012-84f95e060dee?w=640',
        'https://images.unsplash.com/photo-1551446591-142875a901a1?w=640'
      ]
    }
  },

  components: {
  },

  methods: {

  },

  created () {

  }
}
</script>

<style lang='less' scoped>
#home{
  .home-banner{
    color: red;
  }
  .home-cont{
    background: #000;
  }
}
</style>
