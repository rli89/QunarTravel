<template>
  <div class="banner">
    <img class="banner-img" src="https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/CggYGVbNcPKABeNMABAVWGd9g7k807_C_900_504_Q90_Mtg_7.jpg_350x240_b85d103e.jpg" />
    <div class="banner-info">
      <div class="banner-tittle">
        Auckland Musemum
      </div>
      <div class="banner-number">
        <span class="iconfont banner-icon">&#xe692;</span>
        4
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DetailBanner'
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
