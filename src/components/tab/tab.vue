<template>
  <!-- tab组件下，通过路由router引入四个组件recommend、singer、rank、search组件 -->
  <div class="tab">
      <router-link tag="div" to="/recommend" class="tab-item">
        <span class="tab-link">今日推荐</span>
      </router-link>
      <router-link tag="div" to="/flagshipStore" class="tab-item">
        <span class="tab-link">分类</span>
      </router-link>
      <router-link tag="div" to="/rank" class="tab-item">
        <span class="tab-link">新品上线</span>
      </router-link>
      <router-link tag="div" to="/search" class="tab-item">
        <span class="tab-link">搜索</span>
      </router-link>
  </div>
</template>

<script type="text/ecmascript-6">
export default {}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
@import '~common/stylus/variable'

.tab
  display flex
  height 44px
  line-height 44px
  font-size $font-size-medium // 14px字体大小
  border-bottom 1px solid #ddd
  .tab-item
    flex 1
    text-align center
    &.router-link-active // 全局配置 <router-link> 的默认“激活 class 类名
      .tab-link
        // color $color-theme
        // border-bottom 2px solid $color-theme
        padding 6px
        border-radius 3px
        color #fff
        background-color $color-theme
    .tab-link
        padding-bottom 5px
        // color $color-text-l // 灰色
        color $color-text

</style>