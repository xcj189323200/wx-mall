<template>
  <div id='home'>
    <div class="home-banner">
      <swiper class="home-banner-cont">
        <swiper-item  v-for='item in imgUrls' :key="item">
          <image  :src="item" class="slide-image home-banner-img" mode='widthFix'/>
        </swiper-item>
      </swiper>
      <div class="home-banner-btn">
        <h5>立即免费打印</h5> 
      </div>
    </div>
    <div class="home-cont">
      <div class="home-cont-title">
        <i></i>
        <h2>定制美好生活</h2>
      </div>
      <div class="home-cont-con">
        <div class="home-cont-left">
          <div class="home-cont-img"></div>
          <div class="home-cont-img-bttom">
            <h5>5寸高清照片</h5>
            <h6>用时光点亮生活</h6>
            <div><span>¥0.70</span>/张</div>
          </div>
          
        </div>
        <div class="home-cont-right">
          <div class="home-cont-img"></div>
          <div class="home-cont-img-bttom">
            <h5>5寸高清照片</h5>
            <h6>用时光点亮生活</h6>
            <div><span>¥0.70</span></div>
          </div>
          
        </div>
      </div>
      
      
    </div>
    
    
  </div>
</template>

<script>

export default {
  data () {
    return {
      imgUrls: [
        '../../../static/images/home/banner1@2x.png',
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

  margin:0 30rpx;
  background:rgba(240,244,245,1);
  .home-banner{
    width:690rpx;
    height: 510rpx;
    position: relative;
    .home-banner-cont{
      width: 100%;
      height: 510rpx;
    }
    .home-banner-img{
      width:690rpx;
      height: 510rpx
    }
    .home-banner-btn{
      width:300rpx;
      height:84rpx;
      background:linear-gradient(45deg,rgba(255,87,128,1) 0%,rgba(255,195,0,1) 100%);
      border-radius:42rpx;
      text-align:16rpx center;
      position: absolute;
      left: 196rpx;
      top:386rpx;
      h5{
        width:216rpx;
        height:50rpx;
        font-size: 36rpx;
        font-family: PingFangSC-Semibold;
        font-weight:600;
        color: #fff;
        margin-left:42rpx;
        margin-top:16rpx;
      }
    }
  }
  .home-cont{
    position: relative;
    height: 40rpx;
    margin-top:40rpx;
    .home-cont-title{
      
        i{
        width:6rpx;
        height:24rpx;
        background:rgba(255,137,68,1);
        border-radius:3rpx;
        position:absolute;
        top:8rpx;
        display:inline-block;
        margin-right:14rpx
      }
      h2{
        width:168rpx;
        height:40rpx;
        font-size:28rpx;
        font-family:PingFangSC-Regular;
        font-weight:400;
        color:rgba(59,55,53,1);
        line-height:40rpx;
        margin-left:8rpx;
        
      }
    }
    .home-cont-con{
      height: 488rpx;
      .home-cont-left,.home-cont-right{
        width: 334rpx;
        height: 488rpx;
        float: left;
        margin-top: 22rpx;
        .home-cont-img{
          height: 336rpx;
          background:rgba(221,197,197,1);
        }
        .home-cont-img-bttom{
          margin-top:24rpx;
          margin-left: 20rpx;
          h5{
            width:136rpx;
            height:34rpx;
            font-size:24rpx;
            font-weight:500;
            color:rgba(59,55,53,1);
            line-height:34px;
            
          }
          h6{
            width:168rpx;
            height:34rpx;
            font-size:24rpx;
            font-weight:400;
            color:rgba(156,151,149,1);
            line-height:34px;
          }
        }
        
      }
      .home-cont-left{
          margin-right:22rpx;
      }
    }
    
    

  }
  
}
</style>
