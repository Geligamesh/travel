<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe62d;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题</div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe6aa;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style scoped lang="stylus">
  @import '~styles/variables.styl'
  .header
    display: flex
    line-height: .86rem
    background : $bgcolor
    color: #ffffff
    .header-left
      width: .64rem
      float: left
      text-align center
      .back-icon
        text-align center
        font-size .4rem
    .header-input
      flex: 1
      height .64rem
      line-height:.64rem
      margin-top: .11rem
      margin-left: .2rem
      padding-left .2rem
      background: #ffffff
      border-radius: 0.2rem
      color: #ccc

    .header-right
      width: 1.24rem
      float: right
      text-align center
      .arrow-icon
        margin-left -.04rem
        font-size .24rem


</style>
