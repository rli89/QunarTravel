<template>
  <div>
    <div class="location">
      <span class="location-icon"></span>
      location
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
.location
  line-height: .8rem
  font-size: .32rem
  padding: 0 .2rem
</style>
