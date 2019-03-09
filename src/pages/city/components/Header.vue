<template>
  <div class="header">
    <router-link to="/">
      <span class="iconfont arrow-left">&#xe75b;</span>
    </router-link>
    城市选择
  </div>
</template>

<script>

export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varible'
  .header
    position: relative
    background: $bgColor
    color: #fff
    height: .86rem
    line-height: .86rem
    text-align: center
    font-size: .33rem
    .arrow-left
      font-size: .35rem
      position: absolute
      top: 0
      left: 0
      padding-left: .3rem
      color: #fff
</style>
