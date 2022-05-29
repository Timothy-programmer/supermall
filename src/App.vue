<template>
 <div>
   <main-tab-bar></main-tab-bar>

   <router-view></router-view>
 </div>
</template>

<style>
@import "@/assets/css/base.css";
</style>
<script>

import mainTabBar from "@/components/content/mainTabBar/mainTabBar";

export default {
  name:'App',
  components:{
    mainTabBar,

  }
}
</script>
