<template>
  <tab-bar>
    <tab-bar-item :path="'/home'">
      <template #item-icon>
        <img src="@/assets/img/tabbar/home.svg">
      </template>
      <template #item-icon-active>
        <img src="@/assets/img/tabbar/home_active.svg" alt="">
      </template>
      <template #item-text>
        <div slot="item-text">首页</div>
      </template>
    </tab-bar-item>
    <tab-bar-item :path="'/category'">
      <template #item-icon>
        <img src="@/assets/img/tabbar/category.svg">
      </template>
      <template #item-icon-active>
        <img src="@/assets/img/tabbar/category_active.svg" alt="">
      </template>
      <template #item-text>
        <div slot="item-text">分类</div>
      </template>
    </tab-bar-item>
    <tab-bar-item :path="'/cart'">
      <template #item-icon>
        <img src="@/assets/img/tabbar/cart.svg">
      </template>
      <template #item-icon-active>
        <img src="@/assets/img/tabbar/cart_active.svg" alt="">
      </template>
      <template #item-text>
        <div slot="item-text">购物车</div>
      </template>
    </tab-bar-item>
    <tab-bar-item :path="'/profile'">
      <template #item-icon>
        <img src="@/assets/img/tabbar/profile.svg">
      </template>
      <template #item-icon-active>
        <img src="@/assets/img/tabbar/profile_active.svg" alt="">
      </template>
      <template #item-text>
        <div slot="item-text">我的</div>
      </template>
    </tab-bar-item>
  </tab-bar>
</template>

<script>
import TabBar from "@/components/common/tabbar/TabBar";
import TabBarItem from "@/components/common/tabbar/TabBarItem";
export default {
  name: "mainTabBar",
  components:{
    TabBar,
    TabBarItem,
  }
}
</script>

<style scoped>

</style>