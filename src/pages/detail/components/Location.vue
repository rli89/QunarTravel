<template>
<div>
  <div class="location">
    <div class="one border-bottom">
        <span class="location-icon" ></span>
        辽宁省大连市沙河口区中山路608-6-8号星海 ...
    </div>
    <div class="two border-bottom">
        <span class="time-icon"></span>
        查看景点简介及开放时间
    </div>
    <div class="three border-bottom">
      <span class="review-icon"></span>
      4.9分
    </div>
  </div>

</div>
</template>

<script>
export default {
  name: 'DetailLocation',
  props: {
    list: Array
  }
}
</script>

<style lang="stylus" scoped>
.location
  line-height: .8rem
  font-size: .32rem
  padding: 0 .2rem
.location-icon
  position: relative
  left: .06rem
  top: .06rem
  display: inline-block
  width: .36rem
  height: .36rem
  background: url(http://s.qunarzz.com/piao/image/touch/sight/detail.png) 0 -1.80rem no-repeat
  margin-right: .1rem
  background-size: .4rem 3rem
.time-icon
  position: relative
  left: .06rem
  top: .06rem
  display: inline-block
  width: .36rem
  height: .36rem
  background: url(http://s.qunarzz.com/piao/image/touch/sight/detail.png) 0 -2.20rem no-repeat
  margin-right: .1rem
  background-size: .4rem 3rem

.review-icon
  position: relative
  left: .06rem
  top: .06rem
  display: inline-block
  width: .36rem
  height: .36rem
  background: url(http://s.qunarzz.com/piao/image/touch/sight/detail.png) 0 -1.36rem no-repeat
  margin-right: .1rem
  background-size: .4rem 3rem
</style>
