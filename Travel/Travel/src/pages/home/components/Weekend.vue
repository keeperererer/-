<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li
        class="item border-bottom"
        v-for="item of recommendList"
        :key="item.id"
      >
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return{
      recommendList :[{
        id: '0001',
        imgUrl:'http://img1.qunarzz.com/sight/source/1505/fb/302620ed8350f8.jpg_r_640x214_25a07cb4.jpg',
        title:'长沙必游TOP10',
        desc:'到了长沙，一定要到这些地方走走'
      },{
        id: '0002',
        imgUrl:'http://img1.qunarzz.com/sight/source/1505/fb/302620ed8350f8.jpg_r_640x214_25a07cb4.jpg',
        title:'长沙必游TOP10',
        desc:'到了长沙，一定要到这些地方走走'
      },{
        id: '0003',
        imgUrl:'http://img1.qunarzz.com/sight/source/1505/fb/302620ed8350f8.jpg_r_640x214_25a07cb4.jpg',
        title:'长沙必游TOP10',
        desc:'到了长沙，一定要到这些地方走走'
      },{
        id: '0004',
        imgUrl:'http://img1.qunarzz.com/sight/source/1505/fb/302620ed8350f8.jpg_r_640x214_25a07cb4.jpg',
        title:'长沙必游TOP10',
        desc:'到了长沙，一定要到这些地方走走'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 37.09%
    .item-img
      width: 100%
  .item-info
    padding: .1rem
    .item-title
      line-height: .54rem
      font-size: .32rem
      ellipsis()
    .item-desc
      line-height: .4rem
      color: #ccc
      ellipsis()
</style>
