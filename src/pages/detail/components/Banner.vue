<template>
  <div>
    <div class="banner"  @click="handleBannerClick">
        <img class="banner-img" :src="bannerImg"/>
        <div class="banner-info">
        <div class="banner-tittle">
            {{this.sightName}}
        </div>
        <div class="banner-number">
            <span class="iconfont banner-icon">&#xe692;</span>
            {{this.bannerImgs.length}}
        </div>
        </div>
    </div>
    <fade-animation>
      <common-gallary :imgs="bannerImgs"
      v-show="showGallary"
      @close="handleGallaryClose"></common-gallary>
    </fade-animation>

  </div>
</template>

<script>
import CommonGallary from 'common/gallary/Gallary'
import FadeAnimation from '../../../common/fade/FadeAnimation'
export default {
  name: 'DetailBanner',
  props: {
    sightName: String,
    bannerImg: String,
    bannerImgs: Array
  },
  data () {
    return {
      imgs: ['https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/10041f000001gp9gr0BD1_C_900_504.jpg_600x330_a74ae8b8.jpg', 'https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/CggYGVbNcPKABeNMABAVWGd9g7k807_C_900_504_Q90_Mtg_7.jpg_350x240_b85d103e.jpg'],
      showGallary: false
    }
  },
  methods: {
    handleBannerClick () {
      this.showGallary = true
    },
    handleGallaryClose () {
      this.showGallary = false
    }
  },
  components: {
    CommonGallary,
    FadeAnimation
  }
}
</script>

<style lang="stylus" scoped>
  .banner
    overflow: hidden
    height: 0
    padding-bottom: 55%
    position: relative
    .banner-img
      width: 100%
    .banner-info
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #fff
      background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8))
      .banner-tittle
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        height: .32rem
        line-height: .32rem
        margin-top: .14rem
        padding: 0 .4rem
        border-radius: .2rem
        background: rgba(0, 0, 0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
