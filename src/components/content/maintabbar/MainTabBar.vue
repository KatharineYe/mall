<template>
  <div id='main-tab-bar'>
    <div>
      <tab-bar>
        <tab-bar-item path='/home'>
          <span slot="item-text">首页</span>
          <img slot="item-icon"  src='~assets/img/tabbar/home.svg'>
          <img slot="item-icon-active"  src='~assets/img/tabbar/home_active.svg'>
        </tab-bar-item>
        <tab-bar-item path='/category'>
          <span slot="item-text">分类</span>
          <img slot="item-icon"  src='~assets/img/tabbar/category.svg'>
          <img slot="item-icon-active"  src='~assets/img/tabbar/category_active.svg'>
        </tab-bar-item>
        <tab-bar-item path='/shopcart'>
          <span slot="item-text">购物车</span>
          <img slot="item-icon"  src='~assets/img/tabbar/shopcart.svg'>
          <img slot="item-icon-active"  src='~assets/img/tabbar/shopcart_active.svg'>
        </tab-bar-item>
        <tab-bar-item path='/profile'>
          <span slot="item-text">我的</span>
          <img slot="item-icon"  src='~assets/img/tabbar/profile.svg'>
          <img slot="item-icon-active"  src='~assets/img/tabbar/profile_active.svg'>
        </tab-bar-item>
      </tab-bar>
    </div>
  </div>
</template>

<script>
import TabBar from 'components/common/tabbar/TabBar'
import TabBarItem from 'components/common/tabbar/TabBarItem'
export default {
  name: 'MainTabBar',
  data () {
    return {
    }
  },
  methods: {
  },
  computed: {
  },
  components: {
    TabBar,
    TabBarItem
  }
}
</script>

<style scoped>
</style>
