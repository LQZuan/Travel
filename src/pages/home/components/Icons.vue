<template>
    <div class="icons">
        <div class="icon" v-for="item in iconList" :key="item.id">
            <div class="icon-des">
                <div class="iconfont icon-img">&#xe659;</div>
                <p class="icon-img-content">{{item.des}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      iconList: [
        {
          id: '001',
          code: '&#xe659;',
          des: '签证'
        },
        {
          id: '002',
          code: '&#xe76c;',
          des: '出境游'
        },
        {
          id: '003',
          code: '&#xe619;',
          des: '一日游'
        },
        {
          id: '004',
          code: '&#xe60a;',
          des: '美食林'
        },
        {
          id: '005',
          code: '&#xe608;',
          des: '汽车票'
        },
        {
          id: '006',
          code: '&#xe664;',
          des: '邮轮游'
        },
        {
          id: '007',
          code: '&#xe608;',
          des: '超级巴士'
        },
        {
          id: '008',
          code: '&#xe73b;',
          des: '攻略'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .icons
    width: 100%
    overflow: hidden
    height: 0
    padding-bottom: 50%
    // background-color: green
    .icon
      position: relative
      overflow: hidden
      height: 0
      float: left
      width: 25%
      padding-bottom: 25%
      // background-color: red
      box-sizing: border-box
      .icon-des
        position: absolute
        top: 16px
        left: 26px
        text-align: center
        // font-size: .3rem
      .icon-img
        font-size: .8rem
        padding-bottom: .2rem
        // line-height: 100%
      // .icon-img-content
        // height: 100%
</style>
