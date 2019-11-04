<template>
  <tab-bar>
    <tab-bar-item path="/home" activeColor="#ff5777">
      <!-- src 这里的路径使用路径别名需要在别名前加一个 ~ 符号 -->
      <img src="~assets/img/tabbar/home.svg" slot="item-icon" />
      <img src="~assets/img/tabbar/home_active.svg" slot="item-icon-active" />
      <div slot="item-text">首页</div>
    </tab-bar-item>
    <tab-bar-item path="/category" activeColor="#ff5777">
      <img src="~assets/img/tabbar/category.svg" slot="item-icon" />
      <img src="~assets/img/tabbar/category_active.svg" slot="item-icon-active" />
      <div slot="item-text">分类</div>
    </tab-bar-item>
    <tab-bar-item path="/shopcart" activeColor="#ff5777">
      <img src="~assets/img/tabbar/shopcart.svg" slot="item-icon" />
      <img src="~assets/img/tabbar/shopcart_active.svg" slot="item-icon-active" />
      <div slot="item-text">购物车</div>
    </tab-bar-item>
    <tab-bar-item path="/profile" activeColor="#ff5777">
      <img src="~assets/img/tabbar/profile.svg" slot="item-icon" />
      <img src="~assets/img/tabbar/profile_active.svg" slot="item-icon-active" />
      <div slot="item-text">我的</div>
    </tab-bar-item>
  </tab-bar>
</template>

<script>
// import 这里的路径可以直接使用路径别名即可
import TabBar from 'components/common/tabbar/Tabbar'
import TabBarItem from 'components/common/tabbar/TabBarItem'

export default {
  name: 'MainTabBar',
  components: {
    TabBar,
    TabBarItem
  }
}
</script>