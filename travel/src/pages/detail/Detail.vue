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
    DetailList,
    DetailHeader,
    DetailBanner
  },
  data () {
    return {
      list: [{
        title: '成人票',
        children: [{
          title: '成人三馆联票',
          children: [{
            title: '成人三馆联票 - zz旅行社'
          }]
        }, {
          title: '成人五馆联票'
        }]
      }, {
        title: '学生票'
      }, {
        title: '学生票'
      }, {
        title: '特惠票'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .content
    height: 20rem
</style>
