<template>
  <div>
    <detail-banner></detail-banner>
    <detail-header></detail-header>
    <div class="content">
      <detail-list :list="list"></detail-list>
    </div>
  </div>
</template>

<script>
import DetailBanner from './components/Banner'
import DetailHeader from './components/Header'
import DetailList from './components/List'
export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader,
    DetailList
  },
  data () {
    return {
      list: [{
        title: 'Adult Ticket',
        children: [{
          title: 'Adult Combo Ticket',
          children: [{
            title: 'Alibaba Ticket'
          }]
        }, {
          title: 'five Combo'
        }]
      }, {
        title: 'Student Ticket'
      }, {
        title: 'Child Ticket'
      }, {
        title: 'Sale Ticket'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.content
  height:50rem
</style>
