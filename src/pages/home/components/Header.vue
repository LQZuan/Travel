<template>
  <div class="header">
    <router-link to="/city">
      <div class="header-left">
          广州
        <span class="iconfont arrow-icon">&#xe64a;</span>
      </div>
    </router-link>

    <div class="header-input">
      <span class="iconfont">&#xe62d;</span>
      搜索旅游地/酒店/景点
    </div>
    <div class="header-right">
      <div class="iconfont back-icon">&#xe70a;</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varible'
  .header
      line-height: .86rem
      display: flex
      background: $bgColor
      color: #fff
      .header-left
          width: 1.24rem
          float: left
          text-align: center
          color: #fff
          .arrow-icon
              font-size: .2rem
      .header-input
          flex: 1
          height: .64rem
          line-height: .64rem
          margin-top: .12rem
          background: #fff
          color: #ccc
          border-radius: .1rem
      .header-right
          width: .64rem
          float: right
          .back-icon
              text-align: center
              font-size: .4rem
</style>
