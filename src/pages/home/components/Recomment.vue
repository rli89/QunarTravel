<template>
  <div>
    <div class="title">Top Attractions List</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommentList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">Click for details</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecomment',
  data () {
    return {
      recommentList: [{
        id: '0001',
        imgUrl: 'https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/10041f000001gp9gr0BD1_C_900_504.jpg_600x330_a74ae8b8.jpg',
        title: 'Auckland Museum',
        desc: 'The Auckland Museum, also known as the Auckland War Memorial Museum, has been described as a touchstone of the culture and spirit of New Zealanders. It is not only a museum showing the history and culture of the Maori people, but also a war memorial reflecting the history of World War II. '
      }, {
        id: '0002',
        imgUrl: 'https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/100n0m000000djo4x16F3_C_900_504.jpg_600x330_abbc76d8.jpg',
        title: 'Sky Tower',
        desc: 'The Sky Tower is 328 metres high and is an Auckland landmark. It is integrated with other buildings to form a huge sky city. The Sky Tower has three transparent elevators that rise at 18 km/h and take you to the top observation deck and rotating restaurant in just 40 seconds, where you can look down on Auckland like an angel. It is recommended to choose the evening past, first to see a beautiful sunset, as night falls, you can also overlook the night scene of Auckland. In addition, you can experience the sky walk. The Sky Tower Walk is a high-altitude walk on the 192-meter-high outer ring platform of the Sky Tower, led and guided by an instructor.'
      }, {
        id: '0003',
        imgUrl: 'https://qimgs.qunarzz.com/piao_qsight_provider_piao_qsight_web/100s12000000s603s27EA_C_900_504.jpg_350x240_129f6e31.jpg',
        title: 'The Hobbit Village',
        desc: 'The Hobbit Village was the filming location for the Lord of the Rings movie. There are currently 44 Hobbit caves, each with a unique design and artisans taking care of them every day. Take the guided bus at the entrance and you will not only see the Welcome sign "Welcome to Hobbiton" at the entrance, but also admire the verdish-green hillside, the mirrorlike lake and the hobbit hut. Cross stone arched Bridges, mountain paths, hedges and gardens, past the rolling mill, and you will come to the Green Dragon Tavern. The pub is completely restored to the look of the movie, you can not only enjoy a glass of pure non-alcoholic ginger beer here, but also enjoy a delicious lunch or dinner.'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
