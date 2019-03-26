<template>
  <div id='goodsDetails'>
      <div class="goods_banner">
          <swiper class="goods_swiper" indicator-dots="true" autoplay="true" interval="3000">
            <swiper-item  v-for='item in imgUrls' :key="item">
              <image  :src="item" class="goods_swiper_img" mode='widthFix'/>
            </swiper-item>
        </swiper>
        <!--<img src="../../../static/images/goods/20190323162858.png" class="goods_banner-image" mode='widthFix'>-->
        <span class="img_index">111</span>
      </div>
      <div class="price_box">
          <div class="img_size_desc">5寸高清照片</div>
          <div class="img_onsale_price">
            <span class="onsale_price_color">¥0.70</span>
            <span>/张</span>
            <span class="img_orig_price">
            ¥2/张
            </span>
          </div>
          <div class="img_if_hot">热销</div>
      </div>
      <div class="my_coupon">
        <img src="" alt="">
        <span>我的优惠</span>
        <span>免费打印十张</span>
        <img src="" alt="">
      </div>
      <div class="reviews">
        <img src="" alt="">
        <p>评价</p>
        <ul>
          <li>
            <img src="" alt="">
            <p>静候缘来</p>
            <img src="" alt="">
            <p>这是内容</p>
          </li>
        </ul>
        <p>查看更多相关评论</p>
      </div>
      <div class="big_img_box">
        <img src="" alt="">
        <p>立即免费打印</p>
      </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      imgUrls: [
        '../../../static/images/goods/20190323162858.png',
        '../../../static/images/goods/QQ20190323-235604@2x.png'
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
#goodsDetails{
  width:100%;
  background:rgba(240,244,245,1);
  .goods_banner{
      width:750rpx;
      height:750rpx;
      position: relative;
      .goods_swiper{
      width:750rpx;
      height:750rpx;
      .goods_swiper_img{
        width:750rpx;
        height:750rpx;
      }
    }
    .img_index{
      width:56rpx;
      height:44rpx;
      font-size: 24rpx;
      position: absolute;
      bottom: 20rpx;
      right:30rpx;
      background:rgba(59,55,53,0.5);
      color:#FFFFFF;
      text-align:center;
      line-height: 44rpx;
      border:0;
    }
  }
  .price_box{
    width: 750rpx;
    height:194rpx;
    background:rgba(255,255,255,1);
    font-size:24rpx;
    font-family:PingFangSC-Regular;
    font-weight:400;
    color:rgba(156,151,149,1);
    line-height:28rpx;
    margin-top: 0;
    //position: absolute;
    overflow: hidden;
    //background: red;
    .img_size_desc {
      color:#3B3735;
      width:158rpx;
      height:40rpx;
      margin-left: 28rpx;
      margin-top: 30rpx;
      font-size: 28rpx;
      text-align: center;
      line-height: 40rpx;
      font-family: PingFangSC-Regular;
      //position: absolute;
    }
    .img_onsale_price{
      // width: 134rpx;
      height: 40rpx;
      font-size:24rpx;
      font-family:SFProDisplay-Semibold;
      font-weight:600;
      color:rgba(156,151,149,1);
      //display:inline;
      //float: left;
      margin-left: 28rpx;
      margin-top: 6rpx;
      line-height: 40rpx;
      .onsale_price_color{
        font-size: 34rpx;
        color:#FF8944;
        line-height:40rpx;
      }
    }
    .img_orig_price{
      width:100rpx;
      height:34rpx;
      font-size:24rpx;
      font-family:SFProDisplay-Semibold;
      font-weight:600;
      color:rgba(156,151,149,1);
      line-height:28rpx;
      margin-left: 20rpx;
      margin-top: 11rpx;
      text-decoration:line-through;
    }
    .img_if_hot{
      width:66rpx;
      height:42rpx;
      border-radius:4rpx;
      border:2rpx solid rgba(255,137,68,1);
      text-align: center;
      font-size:22rpx;
      font-family:PingFangSC-Regular;
      font-weight:400;
      color:rgba(255,137,68,1);
      line-height:42rpx;
      //clear: both;
      margin-left: 30rpx;
      margin-top: 2rpx;
    }
  }
  .my_coupon{
    width:750rpx;
    height:90rpx;
    margin-top: 20rpx;
    display: inline;
  }
  .reviews{
    width:750rpx;
    height:1068rpx;
  }
  .big_img_box{
    width:750rpx;
    height:5084rpx;
  }
}
</style>
